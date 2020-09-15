---
title: Probleme bei der Anmeldung bei Microsoft 365-apps
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
- "9000571"
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695178"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="2c866-102">Beheben von Microsoft 365-Apps "vertrauenswürdige Plattformmodul Ihres Computers funktioniert nicht ordnungsgemäß"-Meldung</span><span class="sxs-lookup"><span data-stu-id="2c866-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="2c866-103">Um diesen Fehler zu beheben, versuchen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="2c866-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="2c866-104">Installieren Sie die neuesten Updates für [Windows](https://support.microsoft.com/help/4027667/windows-10-update) und [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="2c866-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="2c866-105">[Löschen Sie Office-Anmeldeinformationen](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) mit dem Windows-Anmelde Informations Manager.</span><span class="sxs-lookup"><span data-stu-id="2c866-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="2c866-106">**Hinweis:** Die Registrierungspfade für Office 2016 haben sich in 16,0 geändert.</span><span class="sxs-lookup"><span data-stu-id="2c866-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="2c866-107">(Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="2c866-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="2c866-108">Versuchen Sie den [Benutzer Wiederherstellungsprozess](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) zum Beheben von TPM-Fehlern (Trusted Platform Module).</span><span class="sxs-lookup"><span data-stu-id="2c866-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="2c866-109">Legen Sie die EnableADAL = 0 mit den folgenden Schritten fest:</span><span class="sxs-lookup"><span data-stu-id="2c866-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="2c866-110">Klicken Sie mit der rechten Maustaste auf die Windows-Start Schaltfläche, wählen Sie **Ausführen**, geben Sie **Regedit**ein, und klicken Sie dann auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="2c866-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="2c866-111">Wählen Sie **Ja** aus, um den Registrierungs-Editor zu erlauben, Änderungen an Ihrem Gerät vorzunehmen.</span><span class="sxs-lookup"><span data-stu-id="2c866-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="2c866-112">Fügen Sie im Registrierungs-Editor den DWORD-Wert **EnableADAL** mit der Einstellung **0** unter HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.</span><span class="sxs-lookup"><span data-stu-id="2c866-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="2c866-113">Weitere Informationen finden Sie unter [Verbindungsprobleme bei der Anmeldung nach der Aktualisierung Office 2016 Build 16.0.7967 unter Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="2c866-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>