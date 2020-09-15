---
title: Installieren von Office auf einem Terminal Server-nicht lizenziert
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663116"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="44ae2-102">Installieren von Office auf einem Terminal Server</span><span class="sxs-lookup"><span data-stu-id="44ae2-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="44ae2-103">Für die Bereitstellung von Microsoft 365-Apps für Enterprise auf einem Windows-Server mit Remote Desktop Diensten (RDS), früher benannte Terminal Dienste:</span><span class="sxs-lookup"><span data-stu-id="44ae2-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="44ae2-104">Sie benötigen ein Microsoft 365-Abonnement, das Microsoft 365-Apps für Unternehmen wie Office 365 Enterprise E3 oder Enterprise E5 enthält.</span><span class="sxs-lookup"><span data-stu-id="44ae2-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="44ae2-105">Die Microsoft 365 apps for Business-und Microsoft 365-Apps für Business-Premium-Pläne enthalten keine Microsoft 365-Apps für Enterprise.</span><span class="sxs-lookup"><span data-stu-id="44ae2-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="44ae2-106">Sie müssen die [Aktivierung gemeinsam genutzter Computer](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)aktivieren.</span><span class="sxs-lookup"><span data-stu-id="44ae2-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="44ae2-107">Wenn Sie Microsoft 365-Apps für Enterprise im RDS aus dem Microsoft 365 Admin Center installieren möchten, in dem die ***Standardinstallationseinstellungen verwendet***werden, führen Sie die folgenden Schritte aus.</span><span class="sxs-lookup"><span data-stu-id="44ae2-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="44ae2-108">Sie können den [Microsoft-Support-und Wiederherstellungs-Assistenten](https://aka.ms/SaRA_OfficeSCA_M365Portal) auch herunterladen und ausführen, um Microsoft 365-Apps für Enterprise im freigegebenen Computer Aktivierungsmodus zu installieren.</span><span class="sxs-lookup"><span data-stu-id="44ae2-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="44ae2-109">Überprüfen Sie, welches Microsoft 365-Abonnement Sie haben.</span><span class="sxs-lookup"><span data-stu-id="44ae2-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="44ae2-110">Erfahren Sie, wie</span><span class="sxs-lookup"><span data-stu-id="44ae2-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="44ae2-111">Wechseln Sie bei Bedarf zu einem anderen Microsoft 365-Abonnement.</span><span class="sxs-lookup"><span data-stu-id="44ae2-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="44ae2-112">Erfahren Sie, wie</span><span class="sxs-lookup"><span data-stu-id="44ae2-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="44ae2-113">Wenn Office bereits auf dem RDS-Server mit anderen Microsoft 365-Abonnements installiert ist, deinstallieren Sie es.</span><span class="sxs-lookup"><span data-stu-id="44ae2-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="44ae2-114">Wenn Sie beispielsweise zur Systemsteuerung wechseln, \> deinstallieren Sie ein Programm.</span><span class="sxs-lookup"><span data-stu-id="44ae2-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="44ae2-115">Deinstallieren Sie mit dem [Microsoft-Support-und Wiederherstellungs-Assistenten,](https://aka.ms/SARA-OfficeUninstall-Alchemy) wenn Probleme auftreten.</span><span class="sxs-lookup"><span data-stu-id="44ae2-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="44ae2-116">Melden Sie sich auf dem RDS-Server beim Microsoft 365 Admin Center mit Ihrem Administratorkonto an, und [Installieren Sie Microsoft 365 apps for Enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="44ae2-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="44ae2-117">***Öffnen oder melden*** Sie sich nach der Installation von Office nicht bei Office-Anwendungen an.</span><span class="sxs-lookup"><span data-stu-id="44ae2-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="44ae2-118">Aktivieren Sie auf dem RDS-Server die Aktivierung freigegebener Computer durch Bearbeiten der Registrierung, indem Sie die folgenden Schritte ausführen:</span><span class="sxs-lookup"><span data-stu-id="44ae2-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="44ae2-119">Klicken Sie mit der rechten Maustaste auf die Windows-Schaltfläche in der unteren linken Ecke des Bildschirms, und wählen Sie ausführen aus.</span><span class="sxs-lookup"><span data-stu-id="44ae2-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="44ae2-120">Geben Sie im Feld Öffnen den **Befehl regedit**ein, und wählen Sie dann OK aus.</span><span class="sxs-lookup"><span data-stu-id="44ae2-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="44ae2-121">Wählen Sie ja aus, wenn Sie dazu aufgefordert werden, dass der Registrierungs-Editor Änderungen an Ihrem Gerät vorzunehmen hat.</span><span class="sxs-lookup"><span data-stu-id="44ae2-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="44ae2-122">Fügen Sie im Registrierungs-Editor einen Zeichenfolgenwert von **SharedComputerLicensing** mit der Einstellung 1 unter HKEY_LOCAL_MACHINE \Software\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="44ae2-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="44ae2-123">Melden Sie sich auf dem RDS-Server ***als Endbenutzer an*** , und [Stellen Sie sicher, dass die Aktivierung gemeinsam genutzter Computer für Microsoft 365 apps for Enterprise aktiviert ist](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="44ae2-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="44ae2-124">Ausführliche Informationen zu Voraussetzungen, Setupanweisungen und Anleitungen für benutzerdefinierte Installationen mithilfe des Office-Bereitstellungstools finden Sie unter [Deploy Microsoft 365 apps for Enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="44ae2-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="44ae2-125">Informationen zum Beheben von Fehlern im Zusammenhang mit der Aktivierung gemeinsam genutzter Computer finden Sie unter [Beheben von Problemen mit der Aktivierung gemeinsam genutzter Computer für Microsoft 365 apps for Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="44ae2-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  