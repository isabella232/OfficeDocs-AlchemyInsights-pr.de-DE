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
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="c14f4-102">Probleme bei der Anmeldung bei Office-Apps</span><span class="sxs-lookup"><span data-stu-id="c14f4-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="c14f4-103">Versuchen Sie Folgendes, um Anmeldeprobleme mit Office-Apps zu beheben:</span><span class="sxs-lookup"><span data-stu-id="c14f4-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="c14f4-104">Entfernen Sie alle Arbeits Konten außer dem betroffenen Konto mithilfe von Windows-Einstellungen #a0 **Access work oder School**.</span><span class="sxs-lookup"><span data-stu-id="c14f4-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="c14f4-105">[Löschen Sie Office-Anmeldeinformationen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) mit dem Windows-Anmelde Informations Manager.</span><span class="sxs-lookup"><span data-stu-id="c14f4-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="c14f4-106">**Hinweis:** Die Registrierungspfade für Office 2016 haben sich in 16,0 geändert.</span><span class="sxs-lookup"><span data-stu-id="c14f4-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="c14f4-107">(Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="c14f4-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="c14f4-108">Öffnen Sie eine Office-App, und wählen Sie **Datei** > **Konto** > **Abmelden aus**. Melden Sie sich dann mit einem Benutzerkonto mit einer gültigen Lizenz an.</span><span class="sxs-lookup"><span data-stu-id="c14f4-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="c14f4-109">Ausführliche Informationen finden Sie unter [Konten in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="c14f4-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="c14f4-110">Für Mac finden Sie unter [CAN 't Sign in an an a Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="c14f4-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="c14f4-111">Wenn die Fehler beim Herstellen einer Verbindung mit Office 365 mithilfe von Office 2013 auftreten, aktivieren Sie die moderne Authentifizierung für Office-Client.</span><span class="sxs-lookup"><span data-stu-id="c14f4-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="c14f4-112">Weitere Informationen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="c14f4-112">For more information, see:</span></span>
- [<span data-ttu-id="c14f4-113">Sie können sich nicht bei Office 365, Azure oder InTune anmelden.</span><span class="sxs-lookup"><span data-stu-id="c14f4-113">You can't sign in to Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="c14f4-114">Verbindungsprobleme in der Anmeldung nach der Aktualisierung auf Office 2016 Build 16.0.7967 unter Windows 10</span><span class="sxs-lookup"><span data-stu-id="c14f4-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="c14f4-115">"Es tut uns leid, ein anderes Konto aus Ihrer Organisation ist bereits auf diesem Computer angemeldet" in Office</span><span class="sxs-lookup"><span data-stu-id="c14f4-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="c14f4-116">Behandeln von Anmeldeproblemen mit der modernen Office-Authentifizierung bei Verwendung von ADFS</span><span class="sxs-lookup"><span data-stu-id="c14f4-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)