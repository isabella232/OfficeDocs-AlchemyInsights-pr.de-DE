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
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="0f655-102">Fehler beim Beheben der Office-Apps "Ihr Konto ist in einem schlechten Zustand"</span><span class="sxs-lookup"><span data-stu-id="0f655-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="0f655-103">Um diesen Fehler zu beheben, führen Sie die folgenden Optionen auf dem betroffenen Computer aus:</span><span class="sxs-lookup"><span data-stu-id="0f655-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="0f655-104">Öffnen Sie eine Office-App, und wählen Sie **Datei** > **Konto** > **Abmelden aller Konten aus**.</span><span class="sxs-lookup"><span data-stu-id="0f655-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="0f655-105">Melden Sie sich erneut mit einem Benutzerkonto mit gültiger Lizenz an.</span><span class="sxs-lookup"><span data-stu-id="0f655-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="0f655-106">Ausführliche Informationen finden Sie unter [Konten in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="0f655-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="0f655-107">[Löschen Sie Office-Anmeldeinformationen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) mit dem Windows-Anmelde Informations Manager.</span><span class="sxs-lookup"><span data-stu-id="0f655-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="0f655-108">**Hinweis:** Die Registrierungspfade für Office 2016 haben sich in 16,0 geändert.</span><span class="sxs-lookup"><span data-stu-id="0f655-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="0f655-109">Beispiel: \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="0f655-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="0f655-110">Legen Sie auf dem betroffenen Computer die EnableADAL = 0 mit den folgenden Schritten fest:</span><span class="sxs-lookup"><span data-stu-id="0f655-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="0f655-111">Klicken Sie mit der rechten Maustaste auf die Windows-Schaltfläche, und wählen Sie **Ausführen**.</span><span class="sxs-lookup"><span data-stu-id="0f655-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="0f655-112">Geben Sie im Feld **Öffnen** den **Befehl regedit**ein, und wählen Sie dann **OK**aus.</span><span class="sxs-lookup"><span data-stu-id="0f655-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="0f655-113">Wählen Sie **Ja** aus, wenn Sie dazu aufgefordert werden, dass der Registrierungs-Editor Änderungen an Ihrem Gerät vorzunehmen hat.</span><span class="sxs-lookup"><span data-stu-id="0f655-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="0f655-114">Fügen Sie im Registrierungs-Editor den DWORD-Wert EnableADAL mit der Einstellung 0 unter HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.</span><span class="sxs-lookup"><span data-stu-id="0f655-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="0f655-115">Wenn der Fehler beim Herstellen einer Verbindung mit Office 365 mithilfe von Office 2013 auftritt, aktivieren Sie die [moderne Authentifizierung](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) für den Office-Client.</span><span class="sxs-lookup"><span data-stu-id="0f655-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="0f655-116">Weitere Informationen finden Sie unter [Behandeln von nicht-Browser-apps, die sich nicht bei Office 365, Azure oder InTune anmelden können](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="0f655-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

