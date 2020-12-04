---
title: Problembehandlung bei PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571878"
---
# <a name="troubleshoot-prt-issue"></a>Problembehandlung bei PRT

Damit ein Gerät authentifiziert werden kann, muss es vollständig registriert und in gutem Zustand sein und ein primäres Aktualisierungs Token (PRT) abrufen können.

Für den Prozess der Hybriden Azure AD Beitritts Registrierung müssen sich Geräte in einem Unternehmensnetzwerk befinden. Es funktioniert auch über VPN, aber es gibt einige Vorbehalte. Kunden benötigen Unterstützung bei der Problembehandlung bei der Hybrid-Azure AD Anmeldung bei Remote-Arbeitsbedingungen. Hier ist eine Aufschlüsselung dessen, was passiert "unter der Haube" während des Registrierungsprozesses.

**Cloud-Authentifizierungsumgebung (mit Azure AD Kennworthash Synchronisierung oder Pass-Through-Authentifizierung)**

Dieser Registrierungs Fluss wird auch als "Synchronisierungs Beitritt" bezeichnet.

1. Windows 10 ermittelt einen SCP-Eintrag, wenn sich der Benutzer am Gerät anmeldet.
    1. Das Gerät versucht zunächst, Mandanteninformationen aus dem clientseitigen SCP in der Registrierung [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD] abzurufen. Weitere Informationen finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Wenn ein Fehler auftritt, kommuniziert das Gerät mit lokalem Active Directory (AD), um Mandanteninformationen aus dem Dienstverbindungspunkt (Service Connection Points, SCP) zu erhalten. Informationen zum Überprüfen von SCP finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Es wird empfohlen, SCP in der AD zu aktivieren und nur clientseitigen SCP zur erstmaligen Überprüfung zu verwenden.

2. Windows 10 versucht, mit Azure AD im Systemkontext zu kommunizieren, um sich gegen Azure AD zu authentifizieren. Sie können überprüfen, ob das Gerät unter dem Systemkonto auf Microsoft-Ressourcen zugreifen kann, indem Sie das Verbindungsskript Test Geräteregistrierung verwenden.

3. Windows 10 generiert ein selbstsigniertes Zertifikat und speichert es unter dem Computerobjekt im lokalen AD. Dies erfordert eine Sicht auf Domänen Controller.

4. Ein Device-Objekt, das ein Zertifikat besitzt, wird über Azure AD Connect mit Azure AD synchronisiert. Der Synchronisierungszyklus ist standardmäßig alle 30 Minuten, hängt jedoch von der Konfiguration Azure AD Connect ab. Weitere Informationen finden Sie in diesem [Dokument](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. In dieser Phase sollten Sie das Betreff-Gerät im Status "Ausstehend" unter Device Blade of Azure Portal sehen können.

6. Bei der nächsten Benutzeranmeldung bei Windows 10 wird die Registrierung abgeschlossen. 

> [!NOTE]
> Wenn Sie sich auf VPN befinden und ein Logoff-Anmeldevorgang die Domänen Konnektivität beendet, können Sie die Registrierung manuell auslösen:
 1. Stellen Sie eine dsregcmd/Join lokal an der Administratoreingabeaufforderung oder Remote über PSExec auf Ihrem PC aus. Beispiel: psexec-s \\ win10client01 cmd, dsregcmd/Join

 2. Weitere Informationen zu Problemen mit dem Hybriden Beitritt finden Sie unter Problem [Behandlung bei Geräten](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
