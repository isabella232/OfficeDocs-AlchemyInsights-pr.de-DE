---
title: Installieren von Office auf einem Terminal Server – nicht lizenziert
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 971edd9c064b448446ba16361e99df4a2291c14f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32410121"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="2c602-102">Installieren von Office auf einem Terminal Server</span><span class="sxs-lookup"><span data-stu-id="2c602-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="2c602-103">Für die Bereitstellung von Office 365 proPlus auf einem Windows-Server mit Remote Desktop Dienste (RDS), früher als Terminal Dienste bezeichnet:</span><span class="sxs-lookup"><span data-stu-id="2c602-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="2c602-104">Sie benötigen einen Office 365-Plan mit Office 365 proPlus, wie Office 365 Enterprise E3 oder Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="2c602-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="2c602-105">Die Office 365 Business-und Office 365 Business Premium-Pläne schließen nicht Office 365 proPlus aus.</span><span class="sxs-lookup"><span data-stu-id="2c602-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="2c602-106">Sie müssen die [Aktivierung gemeinsam genutzter Computer](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)aktivieren.</span><span class="sxs-lookup"><span data-stu-id="2c602-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="2c602-107">Führen Sie die folgenden Schritte aus, wenn Sie Office 365 proPlus auf RDS aus dem Office 365-Portal installieren möchten, \* \* *das Standardinstallationseinstellungen* \* \* verwendet:</span><span class="sxs-lookup"><span data-stu-id="2c602-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="2c602-108">Überprüfen Sie, welche Office 365-Plan Sie haben.</span><span class="sxs-lookup"><span data-stu-id="2c602-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="2c602-109">Erfahren Sie, wie</span><span class="sxs-lookup"><span data-stu-id="2c602-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. <span data-ttu-id="2c602-110">Wechseln Sie gegebenenfalls zu einem anderen Office 365-Plan.</span><span class="sxs-lookup"><span data-stu-id="2c602-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="2c602-111">Erfahren Sie, wie</span><span class="sxs-lookup"><span data-stu-id="2c602-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. <span data-ttu-id="2c602-112">Wenn Office bereits auf dem RDS-Server mit anderen Office 365-Plänen installiert ist, deinstallieren Sie es.</span><span class="sxs-lookup"><span data-stu-id="2c602-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="2c602-113">Beispielsweise \> deinstallieren Sie ein Programm in der Systemsteuerung.</span><span class="sxs-lookup"><span data-stu-id="2c602-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="2c602-114">Deinstallieren Sie mit [Microsoft-Support und Wiederherstellungs-Assistent,](https://aka.ms/SARA-OfficeUninstall-Alchemy) wenn Probleme auftreten.</span><span class="sxs-lookup"><span data-stu-id="2c602-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="2c602-115">Melden Sie sich auf dem RDS-Server im Office 365-Portal mit Ihrem Administratorkonto an, und [Installieren Sie Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="2c602-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="2c602-116">Nach der Installation von Office, \* \* *Öffnen Sie nicht oder melden* Sie \* \* für Office-Anwendungen an.</span><span class="sxs-lookup"><span data-stu-id="2c602-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="2c602-117">Aktivieren Sie auf dem RDS-Server die Aktivierung gemeinsam genutzter Computer durch Bearbeiten der Registrierung, indem Sie die folgenden Schritte ausführen:</span><span class="sxs-lookup"><span data-stu-id="2c602-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="2c602-118">Klicken Sie mit der rechten Maustaste in der unteren linken Ecke des Bildschirms auf die Schaltfläche Windows, und wählen Sie ausführen aus.</span><span class="sxs-lookup"><span data-stu-id="2c602-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="2c602-119">Geben Sie im Feld Öffnen den **Befehl regedit**ein, und wählen Sie dann OK aus.</span><span class="sxs-lookup"><span data-stu-id="2c602-119">In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="2c602-120">Wählen Sie ja aus, wenn Sie dazu aufgefordert werden, den Registrierungs-Editor zu ändern.</span><span class="sxs-lookup"><span data-stu-id="2c602-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="2c602-121">Fügen Sie im Registrierungs-Editor einen Zeichenfolgenwert von **SharedComputerLicensing** mit der Einstellung 1 unter HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="2c602-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="2c602-122">Auf dem RDS-Server \* \* *melden* Sie sich als Endbenutzer \* \* an, und [Stellen Sie sicher, dass die Aktivierung gemeinsam genutzter computer für Office 365 ProPlus aktiviert ist](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="2c602-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="2c602-123">Weitere Informationen zu den Voraussetzungen, Setupanweisungen und Anleitungen für angepasste Installationen mithilfe des Office-BereitstellungsTools finden Sie unter [Deploy office 365 ProPlus mithilfe der Remote Desktop Dienste](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="2c602-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="2c602-124">Informationen zur Behebung von Fehlern im Zusammenhang mit der Aktivierung gemeinsam genutzter Computer finden Sie unter [Beheben von Problemen mit der Aktivierung gemeinsam genutzter Computer für Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="2c602-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  

