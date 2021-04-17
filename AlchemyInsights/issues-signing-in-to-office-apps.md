---
title: Probleme bei der Anmeldung bei Microsoft 365-Apps
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
- "9000571"
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833074"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Beheben der Microsoft 365-Apps "Leider ist bereits ein anderes Konto aus Ihrer Organisation angemeldet"

Um diesen Fehler zu beheben, versuchen Sie Folgendes:

- Entfernen Sie alle Arbeitskonten mit Ausnahme des betroffenen Kontos mithilfe von Windows-Einstellungen > **Access-Arbeit oder -Schule**.
- [Löschen von Office-Anmeldeinformationen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) mithilfe von Windows Credential Manager.<br/>
    **Hinweis:** Die Registrierungspfade für Office 2016 wurden auf 16.0 geändert. (Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\)
- Öffnen Sie eine Office-App, wählen **Sie**  >  **Dateikonto**  >  **abmelden aus.** Melden Sie sich dann mit einem Benutzerkonto mit einer gültigen Lizenz an. Ausführliche Informationen finden Sie unter [Konten in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Für Mac lesen Sie [Anmelden bei einer Office 2016 für Mac-App nicht möglich](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Weitere Informationen finden Sie unter "Leider ist ein anderes Konto aus Ihrer Organisation bereits auf diesem Computer [angemeldet" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).