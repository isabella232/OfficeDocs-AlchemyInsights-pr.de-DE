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
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579900"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="db74b-102">Leerer Anmeldebildschirm in Microsoft 365-apps</span><span class="sxs-lookup"><span data-stu-id="db74b-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="db74b-103">Um dieses Problem zu beheben, versuchen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="db74b-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="db74b-104">Installieren Sie die neuesten Updates für [Windows](https://support.microsoft.com/help/4027667/windows-10-update) und [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="db74b-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="db74b-105">Zurücksetzen Internet Explorer Optionen: Wechseln Sie zu **Tools**  >  **Internet Options**  >  **Advanced**  >  **Reset Internet Explorer Settings** (Beachten Sie, dass Sie benutzerdefinierte Einstellungen verlieren), und versuchen Sie dann erneut, sich bei Office anzumelden.</span><span class="sxs-lookup"><span data-stu-id="db74b-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="db74b-106">Deaktivieren Sie den Windows Defender Application Guard (WDAG) oder eine ähnliche Firewall oder ein Antivirus-Programm:</span><span class="sxs-lookup"><span data-stu-id="db74b-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="db74b-107">Wechseln Sie in der Systemsteuerung zu **Programme**, und wählen Sie dann **Windows-Funktionen ein-oder ausschalten aus**.</span><span class="sxs-lookup"><span data-stu-id="db74b-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="db74b-108">Wenn der Windows Defender Application Guard aktiviert ist, deaktivieren Sie ihn.</span><span class="sxs-lookup"><span data-stu-id="db74b-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="db74b-109">**Hinweis:** Möglicherweise müssen Sie den Computer neu starten.</span><span class="sxs-lookup"><span data-stu-id="db74b-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="db74b-110">Stellen Sie sicher, dass das Microsoft. Aad. BrokerPlugin [Aad WAM-Plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nicht von einer Anwendung oder einem Firewall/Anti-Virus-Programm blockiert wird.</span><span class="sxs-lookup"><span data-stu-id="db74b-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="db74b-111">[Löschen Sie Office-Anmeldeinformationen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) mit dem Windows-Anmelde Informations Manager.</span><span class="sxs-lookup"><span data-stu-id="db74b-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="db74b-112">**Hinweis:** Die Registrierungspfade für Office 2016 haben sich in 16,0 geändert.</span><span class="sxs-lookup"><span data-stu-id="db74b-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="db74b-113">(Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="db74b-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="db74b-114">Weitere Informationen finden Sie unter [Verbindungsprobleme bei der Anmeldung nach der Aktualisierung Office 2016 Build 16.0.7967 unter Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="db74b-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>