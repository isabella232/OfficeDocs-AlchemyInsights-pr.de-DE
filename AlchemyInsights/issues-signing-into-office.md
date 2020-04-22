---
title: Probleme bei der Anmeldung bei Office-Apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762998"
---
# <a name="issues-signing-in-to-office-apps"></a>Probleme bei der Anmeldung bei Office-Apps

Versuchen Sie Folgendes, um Anmeldeprobleme mit Office-Apps zu beheben:

- Entfernen Sie alle Arbeits Konten außer dem betroffenen Konto mithilfe von Windows-Einstellungen > **Access work oder School**.
- [Löschen Sie Office-Anmeldeinformationen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) mit dem Windows-Anmelde Informations Manager.<br/>
    **Hinweis:** Die Registrierungspfade für Office 2016 haben sich in 16,0 geändert. (Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\)
- Öffnen Sie eine Office-App, und wählen Sie **Datei** > **Konto** > **Abmelden aus**. Melden Sie sich dann mit einem Benutzerkonto mit einer gültigen Lizenz an. Ausführliche Informationen finden Sie unter [Konten in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Für Mac lesen Sie [Anmelden bei einer Office 2016 für Mac-App nicht möglich](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- Wenn die Fehler beim Herstellen einer Verbindung mit Microsoft 365 mit Office 2013 auftreten, aktivieren Sie die moderne Authentifizierung für Office-Client.

Weitere Informationen finden Sie unter:
- [Sie können sich nicht bei Microsoft 365, Azure oder InTune anmelden.](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Verbindungsprobleme in der Anmeldung nach der Aktualisierung auf Office 2016 Build 16.0.7967 unter Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["Es tut uns leid, ein anderes Konto aus Ihrer Organisation ist bereits auf diesem Computer angemeldet" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [Behandeln von Anmeldeproblemen mit der modernen Office-Authentifizierung bei Verwendung von ADFS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)