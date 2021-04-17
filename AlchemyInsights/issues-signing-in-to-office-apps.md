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
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="ec8a9-102">Beheben der Microsoft 365-Apps "Leider ist bereits ein anderes Konto aus Ihrer Organisation angemeldet"</span><span class="sxs-lookup"><span data-stu-id="ec8a9-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="ec8a9-103">Um diesen Fehler zu beheben, versuchen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="ec8a9-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="ec8a9-104">Entfernen Sie alle Arbeitskonten mit Ausnahme des betroffenen Kontos mithilfe von Windows-Einstellungen > **Access-Arbeit oder -Schule**.</span><span class="sxs-lookup"><span data-stu-id="ec8a9-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="ec8a9-105">[Löschen von Office-Anmeldeinformationen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) mithilfe von Windows Credential Manager.</span><span class="sxs-lookup"><span data-stu-id="ec8a9-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="ec8a9-106">**Hinweis:** Die Registrierungspfade für Office 2016 wurden auf 16.0 geändert.</span><span class="sxs-lookup"><span data-stu-id="ec8a9-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="ec8a9-107">(Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="ec8a9-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="ec8a9-108">Öffnen Sie eine Office-App, wählen **Sie**  >  **Dateikonto**  >  **abmelden aus.** Melden Sie sich dann mit einem Benutzerkonto mit einer gültigen Lizenz an.</span><span class="sxs-lookup"><span data-stu-id="ec8a9-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="ec8a9-109">Ausführliche Informationen finden Sie unter [Konten in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="ec8a9-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="ec8a9-110">Für Mac lesen Sie [Anmelden bei einer Office 2016 für Mac-App nicht möglich](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="ec8a9-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="ec8a9-111">Weitere Informationen finden Sie unter "Leider ist ein anderes Konto aus Ihrer Organisation bereits auf diesem Computer [angemeldet" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="ec8a9-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>