---
title: Probleme bei der Anmeldung bei Microsoft 365-apps
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
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579936"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="c6fc1-102">Beheben der Microsoft 365-Apps "Sorry, ein anderes Konto aus Ihrer Organisation ist bereits angemeldet" Nachricht</span><span class="sxs-lookup"><span data-stu-id="c6fc1-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="c6fc1-103">Um diesen Fehler zu beheben, versuchen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="c6fc1-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="c6fc1-104">Entfernen Sie alle Arbeits Konten außer dem betroffenen Konto mithilfe von Windows-Einstellungen > **Access work oder School**.</span><span class="sxs-lookup"><span data-stu-id="c6fc1-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="c6fc1-105">[Löschen Sie Office-Anmeldeinformationen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) mit dem Windows-Anmelde Informations Manager.</span><span class="sxs-lookup"><span data-stu-id="c6fc1-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="c6fc1-106">**Hinweis:** Die Registrierungspfade für Office 2016 haben sich in 16,0 geändert.</span><span class="sxs-lookup"><span data-stu-id="c6fc1-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="c6fc1-107">(Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="c6fc1-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="c6fc1-108">Öffnen Sie eine Office-App, und wählen Sie **Datei**  >  **Konto**  >  **Abmelden aus**. Melden Sie sich dann mit einem Benutzerkonto mit einer gültigen Lizenz an.</span><span class="sxs-lookup"><span data-stu-id="c6fc1-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="c6fc1-109">Ausführliche Informationen finden Sie unter [Konten in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="c6fc1-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="c6fc1-110">Für Mac lesen Sie [Anmelden bei einer Office 2016 für Mac-App nicht möglich](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="c6fc1-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="c6fc1-111">Weitere Informationen finden Sie unter ["Sorry, ein anderes Konto aus Ihrer Organisation ist bereits auf diesem Computer angemeldet" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="c6fc1-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>