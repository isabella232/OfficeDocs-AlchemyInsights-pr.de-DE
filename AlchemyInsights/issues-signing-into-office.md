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
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938214"
---
# <a name="issues-signing-in-to-office-apps"></a>Probleme bei der Anmeldung bei Office-Apps

Versuchen Sie Folgendes, um Anmeldeprobleme mit Office-Apps zu beheben:

- Entfernen Sie alle Arbeits Konten außer dem betroffenen Konto mithilfe von Windows-Einstellungen #a0 **Access work oder School**.
- [Löschen Sie Office-Anmeldeinformationen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) mit dem Windows-Anmelde Informations Manager.<br/>
    **Hinweis:** Die Registrierungspfade für Office 2016 haben sich in 16,0 geändert. (Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\)
- Öffnen Sie eine Office-App, und wählen Sie **Datei** > **Konto** > **Abmelden aus**. Melden Sie sich dann mit einem Benutzerkonto mit einer gültigen Lizenz an. Ausführliche Informationen finden Sie unter [Konten in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Für Mac finden Sie unter [CAN 't Sign in an an a Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- Wenn die Fehler beim Herstellen einer Verbindung mit Office 365 mithilfe von Office 2013 auftreten, aktivieren Sie die moderne Authentifizierung für Office-Client.

Weitere Informationen finden Sie unter:
- [Sie können sich nicht bei Office 365, Azure oder InTune anmelden.](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Verbindungsprobleme in der Anmeldung nach der Aktualisierung auf Office 2016 Build 16.0.7967 unter Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["Es tut uns leid, ein anderes Konto aus Ihrer Organisation ist bereits auf diesem Computer angemeldet" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [Behandeln von Anmeldeproblemen mit der modernen Office-Authentifizierung bei Verwendung von ADFS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)