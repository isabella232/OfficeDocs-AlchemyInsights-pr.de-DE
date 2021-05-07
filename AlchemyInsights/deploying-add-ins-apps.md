---
title: Bereitstellen von Add-Ins für Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233524"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="d132a-102">Bereitstellen von Add-Ins für Microsoft 365 Apps</span><span class="sxs-lookup"><span data-stu-id="d132a-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="d132a-103">Die zentrale Bereitstellung ist die empfohlene Methode zum Bereitstellen Office Add-Ins für Benutzer und Gruppen in Ihrer Organisation.</span><span class="sxs-lookup"><span data-stu-id="d132a-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="d132a-104">Führen Sie zum Bereitstellen von Add-Ins die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="d132a-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="d132a-105">**Hinweis:** Informationen zum Installieren von Add-Ins für Office benutzer finden Sie unter [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span><span class="sxs-lookup"><span data-stu-id="d132a-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="d132a-106">Stellen Sie außerdem sicher, dass der individuelle Erwerb Office Store Add-Ins aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="d132a-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="d132a-107">Weitere Informationen finden Sie unter [Prevent add-in downloads by off the Office Store across all clients (Except Outlook).](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)</span><span class="sxs-lookup"><span data-stu-id="d132a-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="d132a-108">Stellen Sie sicher, dass Ihre Umgebung die Anforderungen für die Bereitstellung von Add-Ins mithilfe der zentralisierten Bereitstellung erfüllt.</span><span class="sxs-lookup"><span data-stu-id="d132a-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="d132a-109">Weitere Informationen finden Sie unter [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="d132a-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="d132a-110">Wechseln Sie **zu Einstellungen** Integrierte Apps Apps im Microsoft 365 Admin Center zum Bereitstellen  >    >   von Add-Ins.</span><span class="sxs-lookup"><span data-stu-id="d132a-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="d132a-111">Hinweise:</span><span class="sxs-lookup"><span data-stu-id="d132a-111">Notes:</span></span> 

- <span data-ttu-id="d132a-112">Integrierte Apps erfordern, dass der Administrator über globale Administrator- oder Exchange Administratorberechtigungen verfügt.</span><span class="sxs-lookup"><span data-stu-id="d132a-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="d132a-113">Bei der Bereitstellung von Add-Ins für mehrere Benutzer wird empfohlen, Zuweisungen mithilfe von Gruppen anstelle einzelner Benutzer zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="d132a-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="d132a-114">Weitere Informationen finden Sie unter [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span><span class="sxs-lookup"><span data-stu-id="d132a-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="d132a-115">Die zentrale Bereitstellung unterstützt keine Benutzer in geschachtelten Gruppen oder Gruppen mit übergeordneten Gruppen.</span><span class="sxs-lookup"><span data-stu-id="d132a-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="d132a-116">Weitere Informationen finden Sie unter [Benutzer- und Gruppenzuweisungen](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span><span class="sxs-lookup"><span data-stu-id="d132a-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="d132a-117">Stellen Sie sicher, dass der Microsoft 365-App-Verwaltungsdienst (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') für die Anmeldung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="d132a-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="d132a-118">Weitere Informationen finden Sie unter [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span><span class="sxs-lookup"><span data-stu-id="d132a-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="d132a-119">Wenn Probleme beim Bereitstellen von Add-Ins mithilfe von integrierten Apps auftreten, versuchen Sie, die Bereitstellung mithilfe von [Add-Ins zu versuchen.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="d132a-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="d132a-120">Weitere Informationen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="d132a-120">For more information, see:</span></span>

<span data-ttu-id="d132a-121">[Bereitstellen von Add-Ins im Admin Center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Verwalten von Add-Ins im Admin Center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Verwenden der PowerShell-Cmdlets für die zentrale Bereitstellung zum Verwalten von Add-Ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Veröffentlichen Office Add-Ins mithilfe der zentralen Bereitstellung über](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) das Microsoft 365 Admin Center 
 [Problembehandlung: Benutzer sieht keine Add-Ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Behandeln von Benutzerfehlern mit Office-Add-Ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="d132a-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>