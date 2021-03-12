---
title: Probleme bei der Anmeldung bei Microsoft 365-Apps
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
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709105"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="0c601-102">Beheben der Microsoft 365-Apps "Das Modul "Vertrauenswürdige Plattform Ihres Computers funktioniert nicht ordnungsgemäß"</span><span class="sxs-lookup"><span data-stu-id="0c601-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="0c601-103">Um diesen Fehler zu beheben, versuchen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="0c601-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="0c601-104">Installieren Sie die neuesten Updates für [Windows](https://support.microsoft.com/help/4027667/windows-10-update) und [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="0c601-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="0c601-105">[Löschen von Office-Anmeldeinformationen](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) mithilfe von Windows Credential Manager.</span><span class="sxs-lookup"><span data-stu-id="0c601-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="0c601-106">**Hinweis:** Die Registrierungspfade für Office 2016 wurden auf 16.0 geändert.</span><span class="sxs-lookup"><span data-stu-id="0c601-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="0c601-107">(Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="0c601-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="0c601-108">Versuchen Sie den [Benutzerwiederherstellungsprozess,](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) um TPM-Fehler (Trusted Platform Module) zu beheben.</span><span class="sxs-lookup"><span data-stu-id="0c601-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="0c601-109">Legen Sie enableADAL = 0 mithilfe der folgenden Schritte auf:</span><span class="sxs-lookup"><span data-stu-id="0c601-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="0c601-110">Klicken Sie mit der rechten Maustaste auf die Schaltfläche Windows Start, wählen **Sie Ausführen,** **geben Sie regedit** ein, und wählen Sie dann **OK aus.**</span><span class="sxs-lookup"><span data-stu-id="0c601-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="0c601-111">Wählen **Sie Ja** aus, damit der Registrierungs-Editor Änderungen an Ihrem Gerät vornehmen kann.</span><span class="sxs-lookup"><span data-stu-id="0c601-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="0c601-112">Fügen Sie im Registrierungs-Editor einen DWORD-Wert **von EnableADAL** mit der Einstellung **0** unter HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="0c601-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="0c601-113">Weitere Informationen finden Sie unter Verbindungsprobleme bei der Anmeldung nach dem Update auf [Office 2016 Build 16.0.7967 unter Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="0c601-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>