---
title: Installieren von Office auf einem Terminal Server-nicht lizenziert
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: edac051840594f13b22ccd83f5cd6e3da5f84cbc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36498414"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="03c75-102">Installieren von Office auf einem Terminal Server</span><span class="sxs-lookup"><span data-stu-id="03c75-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="03c75-103">Für die Bereitstellung von Office 365 ProPlus auf einem Windows-Server mit Remote Desktop Diensten (RDS), ehemals Terminal Dienste genannt:</span><span class="sxs-lookup"><span data-stu-id="03c75-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="03c75-104">Sie benötigen einen Office 365 Plan mit Office 365 ProPlus, beispielsweise Office 365 Enterprise E3 oder Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="03c75-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="03c75-105">Die Office 365 Business-und Office 365 Business Premium-Pläne enthalten nicht Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="03c75-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="03c75-106">Sie müssen die [Aktivierung gemeinsam genutzter Computer](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)aktivieren.</span><span class="sxs-lookup"><span data-stu-id="03c75-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="03c75-107">Wenn Sie Office 365 ProPlus über das Office 365 Portal, in ***dem standardmäßige Installationseinstellungen verwendet***werden, auf RDS installieren möchten, führen Sie die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="03c75-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, ***which uses default installation settings***, follow these steps:</span></span>
  
1. <span data-ttu-id="03c75-108">Überprüfen Sie, welche Office 365 Plan Sie haben.</span><span class="sxs-lookup"><span data-stu-id="03c75-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="03c75-109">Erfahren Sie, wie</span><span class="sxs-lookup"><span data-stu-id="03c75-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="03c75-110">Wechseln Sie bei Bedarf zu einem anderen Office 365 Plan.</span><span class="sxs-lookup"><span data-stu-id="03c75-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="03c75-111">Erfahren Sie, wie</span><span class="sxs-lookup"><span data-stu-id="03c75-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="03c75-112">Wenn Office bereits auf dem RDS-Server mit anderen Office 365 Plänen installiert ist, deinstallieren Sie es.</span><span class="sxs-lookup"><span data-stu-id="03c75-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="03c75-113">Wenn Sie beispielsweise zur Systemsteuerung wechseln \> , deinstallieren Sie ein Programm.</span><span class="sxs-lookup"><span data-stu-id="03c75-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="03c75-114">Deinstallieren Sie mit dem [Microsoft-Support-und Wiederherstellungs-Assistenten,](https://aka.ms/SARA-OfficeUninstall-Alchemy) wenn Probleme auftreten.</span><span class="sxs-lookup"><span data-stu-id="03c75-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="03c75-115">Melden Sie sich auf dem RDS-Server mit Ihrem Administratorkonto beim Office 365-Portal an, und [Installieren Sie Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="03c75-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="03c75-116">***Öffnen oder melden*** Sie sich nach der Installation von Office nicht bei Office-Anwendungen an.</span><span class="sxs-lookup"><span data-stu-id="03c75-116">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="03c75-117">Aktivieren Sie auf dem RDS-Server die Aktivierung freigegebener Computer durch Bearbeiten der Registrierung, indem Sie die folgenden Schritte ausführen:</span><span class="sxs-lookup"><span data-stu-id="03c75-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="03c75-118">Klicken Sie mit der rechten Maustaste auf die Windows-Schaltfläche in der unteren linken Ecke des Bildschirms, und wählen Sie ausführen aus.</span><span class="sxs-lookup"><span data-stu-id="03c75-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="03c75-119">Geben Sie im Feld Öffnen den **Befehl regedit**ein, und wählen Sie dann OK aus.</span><span class="sxs-lookup"><span data-stu-id="03c75-119">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="03c75-120">Wählen Sie ja aus, wenn Sie dazu aufgefordert werden, dass der Registrierungs-Editor Änderungen an Ihrem Gerät vorzunehmen hat.</span><span class="sxs-lookup"><span data-stu-id="03c75-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="03c75-121">Fügen Sie im Registrierungs-Editor einen Zeichenfolgenwert von **SharedComputerLicensing** mit der Einstellung 1 unter HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="03c75-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="03c75-122">Melden Sie sich auf dem RDS-Server ***als Endbenutzer an*** , und [Stellen Sie sicher, dass die Aktivierung gemeinsam genutzter Computer für Office 365 ProPlus aktiviert ist](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="03c75-122">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="03c75-123">Ausführliche Informationen zu Voraussetzungen, Setupanweisungen und Anleitungen für benutzerdefinierte Installationen mithilfe des Office-Bereitstellungstools finden Sie unter [Deploy Office 365 ProPlus mithilfe von Remote Desktop Dienste](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="03c75-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="03c75-124">Informationen zum Beheben von Fehlern im Zusammenhang mit der Aktivierung gemeinsam genutzter Computer finden Sie unter [Beheben von Problemen mit der Aktivierung gemeinsam genutzter Computer für Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="03c75-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  