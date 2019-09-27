---
title: Datenspeicherort
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207260"
---
# <a name="data-location"></a><span data-ttu-id="a7e73-102">Datenspeicherort</span><span class="sxs-lookup"><span data-stu-id="a7e73-102">Data location</span></span>

<span data-ttu-id="a7e73-103">Sie können den Speicherort des Office 365 Mandanten im Admin Center anzeigen oder über PowerShell eine Verbindung mit Exchange Online herstellen.</span><span class="sxs-lookup"><span data-stu-id="a7e73-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="a7e73-104">**Admin Center:**</span><span class="sxs-lookup"><span data-stu-id="a7e73-104">**Admin center:**</span></span>
1. <span data-ttu-id="a7e73-105">Melden Sie sich beim [Admin Center](https://admin.microsoft.com/Adminportal/Home)an.</span><span class="sxs-lookup"><span data-stu-id="a7e73-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="a7e73-106">Wählen Sie**Organisationsprofil**für **Einstellungen** > aus.</span><span class="sxs-lookup"><span data-stu-id="a7e73-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="a7e73-107">Wählen Sie unter **Datenspeicherort**die Option **Details anzeigen**aus.</span><span class="sxs-lookup"><span data-stu-id="a7e73-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="a7e73-108">**PowerShell**</span><span class="sxs-lookup"><span data-stu-id="a7e73-108">**PowerShell:**</span></span>
1. <span data-ttu-id="a7e73-109">Stellen Sie mithilfe von Windows PowerShell eine Verbindung zu Exchange Online her.</span><span class="sxs-lookup"><span data-stu-id="a7e73-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="a7e73-110">Führen Sie das Cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) aus, um eine Liste der Eigenschaften Ihres Mandanten anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="a7e73-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="a7e73-111">Sehen Sie sich die Organizational-Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="a7e73-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="a7e73-112">Wenn Sie den Datenspeicherort für Exo und SPO haben, können Sie den Datenspeicherort für andere Dienste bestimmen, die Sie von der Stelle aus, an der [sich Ihre Daten befinden](https://products.office.com/where-is-your-data-located), verwenden können.</span><span class="sxs-lookup"><span data-stu-id="a7e73-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>