---
title: Beheben der Office-Apps, die Ihr Konto in einer fehlerhaften Statusmeldung befindet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969451"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Fehler beim Beheben der Office-Apps "Ihr Konto ist in einem schlechten Zustand"

Um diesen Fehler zu beheben, führen Sie die folgenden Optionen auf dem betroffenen Computer aus:

- Öffnen Sie eine Office-App, und wählen Sie **Datei** > **Konto** > **Abmelden aller Konten aus**. Melden Sie sich erneut mit einem Benutzerkonto mit gültiger Lizenz an. Ausführliche Informationen finden Sie unter [Konten in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Löschen Sie Office-Anmeldeinformationen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) mit dem Windows-Anmelde Informations Manager.<br>
  **Hinweis:** Die Registrierungspfade für Office 2016 haben sich in 16,0 geändert. Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\
- Legen Sie auf dem betroffenen Computer die EnableADAL = 0 mit den folgenden Schritten fest:  
     1. Klicken Sie mit der rechten Maustaste auf die Windows-Schaltfläche, und wählen Sie **Ausführen**. Geben Sie im Feld **Öffnen** den **Befehl regedit**ein, und wählen Sie dann **OK**aus.
     2. Wählen Sie **Ja** aus, wenn Sie dazu aufgefordert werden, dass der Registrierungs-Editor Änderungen an Ihrem Gerät vorzunehmen hat.
    3. Fügen Sie im Registrierungs-Editor den DWORD-Wert EnableADAL mit der Einstellung 0 unter HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.
- Wenn der Fehler beim Herstellen einer Verbindung mit Office 365 mithilfe von Office 2013 auftritt, aktivieren Sie die [moderne Authentifizierung](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) für den Office-Client.

Weitere Informationen finden Sie unter [Behandeln von nicht-Browser-apps, die sich nicht bei Office 365, Azure oder InTune anmelden können](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

