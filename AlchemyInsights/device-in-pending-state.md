---
title: Gerät im Zustand "Ausstehend"
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
ms.openlocfilehash: 224e6e613c306b50e354930bcbe6f43f1c08528766cb6e681b0e9826b2d55a4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914002"
---
# <a name="device-in-pending-state"></a>Gerät im Zustand "Ausstehend"

**Voraussetzungen:**

1. Wenn Sie Geräteregistrierungen zum ersten Mal einrichten, stellen Sie sicher, dass Sie die Einführung in die [Geräteverwaltung in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) überprüft haben, die Sie darüber informieren, wie Sie Geräte unter die Kontrolle von Azure AD bringen.
2. Wenn Sie Geräte direkt bei Azure AD registrieren und sie bei Intune registrieren, müssen Sie sicherstellen, dass Sie [Intune konfiguriert](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) und die [Lizenzierung](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) zuerst eingerichtet haben.
3. Stellen Sie sicher, dass Sie berechtigt sind, Vorgänge in Azure AD und lokalem AD auszuführen. Nur ein globaler Administrator in Azure AD kann Einstellungen für Geräteregistrierungen verwalten. Wenn Sie außerdem automatische Registrierungen in Ihrem lokalen Active Directory einrichten, müssen Sie außerdem Administrator von Active Directory und (sofern zutreffend) AD FS sein.

Für den Azure AD-Hybridbeitrittsregistrierungsprozess müssen sich Geräte im Unternehmensnetzwerk befinden. Es funktioniert auch über VPN, aber es gibt einige Einschränkungen. Wir haben gehört, dass Kunden Unterstützung bei der Problembehandlung beim Azure AD-Hybridregistrierungsprozess unter Remotearbeitsumgebungen benötigen.

**Cloudauthentifizierungsumgebung (mit azure AD-Kennworthashsynchronisierung oder Pass-Through-Authentifizierung)**

Dieser Registrierungsfluss wird auch als "Sync Join" bezeichnet.

Nachfolgend sehen Sie eine Aufschlüsselung der Vorgänge während des Registrierungsvorgangs:

1. Windows 10 erkennt den SCP-Eintrag (Service Connection Point), wenn sich der Benutzer am Gerät anmeldet.

    1. Das Gerät versucht zunächst, Mandanteninformationen aus clientseitigem SCP in der Registrierung [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD] abzurufen. Weitere Informationen finden Sie unter [Dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Wenn ein Fehler auftritt, kommuniziert das Gerät mit dem lokalen Active Directory, um Mandanteninformationen von SCP abzurufen. Informationen zum Überprüfen von SCP finden Sie in diesem [Dokument.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)

    > [!NOTE]
    > Es wird empfohlen, SCP in Active Directory zu aktivieren und nur clientseitige SCP für die anfängliche Überprüfung zu verwenden.

2. Windows 10 versucht, mit Azure AD im Systemkontext zu kommunizieren, um sich bei Azure AD zu authentifizieren.

    Sie können überprüfen, ob das Gerät unter dem Systemkonto auf Microsoft-Ressourcen zugreifen kann, indem Sie das [Skript "Geräteregistrierungskonnektivität testen"](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)verwenden.

3. Windows 10 generiert ein selbstsigngeschütztes Zertifikat und speichert es unter dem Computerobjekt im lokalen Active Directory. Dies erfordert eine Sichtachse für den Domänencontroller.

4. Das Geräteobjekt, das über ein Zertifikat verfügt, wird über Azure AD Verbinden mit Azure AD synchronisiert. Der Synchronisierungszyklus erfolgt standardmäßig alle 30 Minuten, hängt jedoch von der Konfiguration der Azure AD-Verbinden ab. Weitere Informationen finden Sie in diesem [Dokument.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. In dieser Phase sollten Sie das Betreffgerät im Status **"Ausstehend"** unter dem Geräteblatt des Azure-Portals sehen können.

6. Bei der nächsten Benutzeranmeldung bei Windows 10 wird die Registrierung abgeschlossen.

    > [!NOTE]
    > Wenn Sie sich auf einem VPN befinden und die Domänenkonnektivität abbricht, können Sie die Registrierung manuell auslösen. Gehen Sie dazu wie folgt vor:
    >
    > Stellen Sie eine `dsregcmd /join` lokale Administratoraufforderung oder remote über PSExec auf Ihrem PC aus.
    >
    > Beispiel: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Allgemeine Probleme mit Azure Active Directory Geräteregistrierung finden Sie unter ["Häufig gestellte Fragen zu Geräten".](https://docs.microsoft.com/azure/active-directory/devices/faq)
