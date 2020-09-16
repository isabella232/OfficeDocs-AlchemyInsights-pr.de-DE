---
title: Beheben der Microsoft 365-apps Ihr Konto befindet sich in einer fehlerhaften Statusmeldung
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744544"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Beheben von Microsoft 365-Apps "Ihr Konto ist in einem fehlerhaften Zustand"

Um diesen Fehler zu beheben, führen Sie die folgenden Optionen auf dem betroffenen Computer aus:

- Öffnen Sie eine Office-App, und wählen Sie **Datei**  >  **Konto**  >  **Abmelden aller Konten aus**. Melden Sie sich mit einem Benutzerkonto mit einer gültigen Lizenz erneut an. Ausführliche Informationen finden Sie unter [Konten in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Löschen Sie Office-Anmeldeinformationen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) mit dem Windows-Anmelde Informations Manager.<br>
  **Hinweis:** Die Registrierungspfade für Office 2016 haben sich in 16,0 geändert. Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\
- Wenn der Fehler beim Herstellen einer Verbindung mit Office 365 mithilfe von Office 2013 auftritt, aktivieren Sie die [moderne Authentifizierung](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) für den Office-Client.

Weitere Informationen finden Sie unter [Behandeln von nicht-Browser-apps, die sich nicht bei Microsoft 365, Azure oder InTune anmelden können](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

