---
title: Herstellen einer Verbindung mit dem MS Commerce-Modul
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 8e6819f6d6ff37baab4bdd49cb5a87c32490f841
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51829735"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a><span data-ttu-id="0c7fa-102">MS Commerce erfordert ein Konto des Unternehmens- oder Abrechnungsadministrators</span><span class="sxs-lookup"><span data-stu-id="0c7fa-102">MSCommerce requires a Company or Billing Administrator account</span></span>

<span data-ttu-id="0c7fa-103">Das MODUL MS Commerce erfordert ein Konto mit Berechtigungen des Unternehmens- oder Abrechnungsadministrators.</span><span class="sxs-lookup"><span data-stu-id="0c7fa-103">The MSCommerce module requires an account with Company or Billing Administrator privileges.</span></span> <span data-ttu-id="0c7fa-104">Wenn Sie den folgenden Fehler erhalten, müssen Sie eine Verbindung mit einem anderen Konto herstellen.</span><span class="sxs-lookup"><span data-stu-id="0c7fa-104">If you are receiving the following error, you will need to reconnect with a different account.</span></span>

<span data-ttu-id="0c7fa-105">*ErrorMessage – Der Remoteserver hat einen Fehler zurückgegeben: (403) Verboten. ErrorDetails - unter C:\Program Files\WindowsPowerShell\Modules\MS Commerce\1.2\MS Commerce.psm1:216 char:5*</span><span class="sxs-lookup"><span data-stu-id="0c7fa-105">*ErrorMessage - The remote server returned an error: (403) Forbidden. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*</span></span><br>
<span data-ttu-id="0c7fa-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Fehler beim Retri...*</span><span class="sxs-lookup"><span data-stu-id="0c7fa-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...*</span></span><br>
<span data-ttu-id="0c7fa-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span><span class="sxs-lookup"><span data-stu-id="0c7fa-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span></span><br>
<span data-ttu-id="0c7fa-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo : NotSpecified: (:) [Write-Error], WriteErrorException*</span><span class="sxs-lookup"><span data-stu-id="0c7fa-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException*</span></span><br>
<span data-ttu-id="0c7fa-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*</span><span class="sxs-lookup"><span data-stu-id="0c7fa-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*</span></span>

<span data-ttu-id="0c7fa-110">Wenn Ihr Konto nicht über Die Rechte des Unternehmens- oder Abrechnungsadministrators verfügt, wenden Sie sich an Ihren IT-Administrator.</span><span class="sxs-lookup"><span data-stu-id="0c7fa-110">If your account does not have Company or Billing Administrator privileges, contact your IT Admin.</span></span>
