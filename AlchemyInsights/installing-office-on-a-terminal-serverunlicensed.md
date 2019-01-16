---
title: Installieren von Office auf einem Terminalserver - nicht lizenzierten
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28289775"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="3c78f-102">Installieren von Office auf einem Terminalserver</span><span class="sxs-lookup"><span data-stu-id="3c78f-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="3c78f-103">Für die Bereitstellung von Office 365 ProPlus auf einem Windows-Server mit Remote Desktop Services (RDS), namens früher Terminaldienste:</span><span class="sxs-lookup"><span data-stu-id="3c78f-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="3c78f-p101">Sie müssen einen Office 365-Plan verfügen, der Office 365 ProPlus, wie Office 365 Enterprise E3 oder Enterprise E5 enthält. Die Office 365 Geschäfts- und Office 365 Business Premium Pläne enthalten nicht Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="3c78f-p101">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5. The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="3c78f-106">Sie müssen [gemeinsam genutzter Computer Aktivierung](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="3c78f-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="3c78f-107">Wenn Sie Office 365 ProPlus über das Office 365-Portal auf RDS installieren möchten \*\* *die Standardeinstellungen für die Installation verwendet* \*\*, gehen Sie folgendermaßen vor:</span><span class="sxs-lookup"><span data-stu-id="3c78f-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="3c78f-p102">Welche Office 365-Plan Sie haben überprüfen. [Erfahren Sie, wie](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span><span class="sxs-lookup"><span data-stu-id="3c78f-p102">Check what Office 365 plan you have. [Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span></span>
    
2. <span data-ttu-id="3c78f-p103">Falls erforderlich, wechseln Sie zu einem anderen Office 365 planen. [Erfahren Sie, wie](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span><span class="sxs-lookup"><span data-stu-id="3c78f-p103">If necessary, switch to a different Office 365 plan. [Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span></span>
    
3. <span data-ttu-id="3c78f-p104">Wenn Office bereits auf dem anderen Office 365-Pläne mit RDS-Server installiert ist, deinstallieren Sie es. Angenommen, indem Sie auf Systemsteuerung \> Programm deinstallieren. Deinstallieren Sie [Microsoft-Support und Recovery-Assistenten](https://aka.ms/SARA-OfficeUninstall-Alchemy) verwenden, wenn Sie Probleme ausführen.</span><span class="sxs-lookup"><span data-stu-id="3c78f-p104">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it. For example, by going to Control Panel \> Uninstall a program. Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="3c78f-115">Melden Sie sich auf dem Server RDS in Office 365-Portal mit Ihrem Administratorkonto und [Installieren von Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)an.</span><span class="sxs-lookup"><span data-stu-id="3c78f-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="3c78f-116">Nach der Installation von Office \*\* *Öffnen oder melden Sie sich nicht* \*\* für alle Office-Clientanwendungen.</span><span class="sxs-lookup"><span data-stu-id="3c78f-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="3c78f-117">Aktivieren Sie auf dem Server RDS gemeinsam genutzter Computer Aktivierung durch Bearbeiten der Registrierung durch die folgenden Schritte ausführen:</span><span class="sxs-lookup"><span data-stu-id="3c78f-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="3c78f-p105">Mit der rechten Maustaste in der unteren linken Ecke des Bildschirms der Windows-Schaltfläche, und wählen Sie ausführen aus. Öffnen Sie im Feld Geben Sie **regedit ein**, und wählen Sie dann auf OK.</span><span class="sxs-lookup"><span data-stu-id="3c78f-p105">Right-click the Windows button in the lower left-hand corner of your screen and select Run. In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="3c78f-120">Wählen Sie Ja bei entsprechender Aufforderung zum Zulassen des Registrierungs-Editor auf Ihrem Gerät ändern.</span><span class="sxs-lookup"><span data-stu-id="3c78f-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="3c78f-121">In den Registrierungs-Editor, fügen einen String-Wert der **SharedComputerLicensing** mit der Einstellung 1 unter HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration hinzu.</span><span class="sxs-lookup"><span data-stu-id="3c78f-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="3c78f-122">Auf dem Server RDS \*\* *Melden Sie sich als Endbenutzer* \*\* und [Stellen Sie sicher, dass gemeinsam genutzter Computer Aktivierung für Office 365 ProPlus aktiviert ist](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="3c78f-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="3c78f-123">Weitere Informationen zu Voraussetzungen, zur Einrichtung und Anleitungen für benutzerdefinierte Installationen mithilfe des Office-Bereitstellungstools Bitte finden Sie unter [Bereitstellen von Office 365 ProPlus mithilfe von Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="3c78f-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="3c78f-124">Zum Beheben von Fehlern im Zusammenhang mit der Aktivierung des freigegebenen finden Sie unter [Troubleshoot Probleme bei der Aktivierung für Office 365 ProPlus gemeinsam genutzter Computer](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="3c78f-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  

