---
title: Gerät im Status "Ausstehend"
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/11/2020
ms.locfileid: "49652188"
---
# <a name="device-in-pending-state"></a>Gerät im Status "Ausstehend"

**Voraussetzungen**

1. Wenn Sie Geräte Registrierungen zum ersten Mal einrichten, stellen Sie sicher, dass Sie die Einführung in die [Geräteverwaltung in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) überprüft haben, in dem Sie erfahren, wie Sie Geräte unter Kontrolle von Azure AD erhalten.
2. Wenn Sie Geräte direkt in Azure AD registrieren und diese in InTune einschreiben, müssen Sie sicherstellen, dass Sie [InTune konfiguriert](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) haben und die [Lizenzierung](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) zuerst eingerichtet haben.
3. Stellen Sie sicher, dass Sie berechtigt sind, Vorgänge in Azure AD und lokalen AD auszuführen. Nur ein globaler Administrator in Azure AD kann Einstellungen für Geräte Registrierungen verwalten. Wenn Sie automatische Registrierungen in Ihrer lokalen Active Directory einrichten, müssen Sie außerdem Administrator von Active Directory und AD FS sein (falls zutreffend).

Für den Prozess der Hybriden Azure AD Beitritts Registrierung müssen sich Geräte im Unternehmensnetzwerk befinden. Es funktioniert auch über VPN, aber es gibt einige Vorbehalte. Wir haben Kunden gehört, die Unterstützung bei der Problembehandlung für den Hybrid-Azure AD Anmeldungsprozess unter Remote-Arbeitsbedingungen benötigen.

**Cloud-Authentifizierungsumgebung (mit Azure AD Kennworthash Synchronisierung oder Pass-Through-Authentifizierung)**

Dieser Registrierungs Fluss wird auch als "Synchronisierungs Beitritt" bezeichnet.

Hier finden Sie eine Aufschlüsselung der Vorgänge während des Registrierungsvorgangs:

1. Windows 10 erkennt den Dienstverbindungspunkt-Eintrag (SCP), wenn sich der Benutzer am Gerät anmeldet.

    1. Das Gerät versucht zunächst, Mandanteninformationen aus dem clientseitigen SCP in der Registrierung [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD] abzurufen. Weitere Informationen finden Sie unter [Document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Wenn ein Fehler auftritt, kommuniziert das Gerät mit lokalem Active Directory, um Mandanteninformationen von SCP zu erhalten. Um SCP zu überprüfen, lesen Sie dieses [Dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Es wird empfohlen, SCP im Active Directory zu aktivieren und nur clientseitigen SCP für die erste Überprüfung zu verwenden.

2. Windows 10 versucht, mit Azure AD im Systemkontext zu kommunizieren, um sich gegen Azure AD zu authentifizieren.

    Sie können überprüfen, ob das Gerät unter dem Systemkonto auf Microsoft-Ressourcen zugreifen kann, indem Sie das [Verbindungsskript Test Geräteregistrierung](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)verwenden.

3. Windows 10 generiert selbstsigniertes Zertifikat und speichert es unter dem Computerobjekt im lokalen Active Directory. Dies erfordert eine Sicht auf Domänen Controller.

4. Das Geräteobjekt, für das das Zertifikat verwendet wird, wird über Azure AD Connect mit Azure AD synchronisiert. Der Synchronisierungszyklus ist standardmäßig alle 30 Minuten, hängt jedoch von der Konfiguration von Azure AD Connect ab. Weitere Informationen finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. In dieser Phase sollten Sie das Betreff-Gerät im Status "**Ausstehend**" unter Device Blade of Azure Portal sehen können.

6. Bei der nächsten Benutzeranmeldung bei Windows 10 wird die Registrierung abgeschlossen.

    > [!NOTE]
    > Wenn Sie sich auf VPN befinden und Logoff/Login die Domänen Konnektivität beendet, können Sie die Registrierung manuell auslösen. Gehen Sie dazu wie folgt vor:
    >
    > Stellen Sie eine `dsregcmd /join` lokale über Administratoreingabeaufforderung oder Remote über PSExec auf Ihrem PC aus.
    >
    > Beispiel: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Häufige Probleme bei der Registrierung von Azure Active Directory-Geräten finden Sie unter [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).
