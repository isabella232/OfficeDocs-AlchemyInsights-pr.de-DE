---
title: Beheben der Microsoft 365-Apps Ihr Konto befindet sich in einer Meldung mit einem schlechten Status
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812535"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Beheben des Microsoft 365-Apps-Fehlers "Ihr Konto befindet sich in einem schlechten Zustand"

Um diesen Fehler zu beheben, testen Sie die folgenden Optionen auf dem betroffenen Computer:

- Öffnen Sie eine Office-App, wählen Sie  >  **Dateikonto**  >  **Abmelden aller Konten aus.** Melden Sie sich mit einem Benutzerkonto mit einer gültigen Lizenz erneut an. Ausführliche Informationen finden Sie unter [Konten in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Löschen von Office-Anmeldeinformationen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) mithilfe von Windows Credential Manager.<br>
  **Hinweis:** Die Registrierungspfade für Office 2016 wurden auf 16.0 geändert. Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\
- Wenn der Fehler beim Herstellen einer Verbindung mit Office 365 mit Office 2013 auftritt, aktivieren Sie [die moderne](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) Authentifizierung für den Office-Client.

Weitere Informationen finden Sie unter Behandeln von [Nicht-Browser-Apps,](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)die sich nicht bei Microsoft 365, Azure oder Intune anmelden können.

