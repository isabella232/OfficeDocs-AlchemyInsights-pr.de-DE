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
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MS Commerce erfordert ein Konto des Unternehmens- oder Abrechnungsadministrators

Das MODUL MS Commerce erfordert ein Konto mit Berechtigungen des Unternehmens- oder Abrechnungsadministrators. Wenn Sie den folgenden Fehler erhalten, müssen Sie eine Verbindung mit einem anderen Konto herstellen.

*ErrorMessage – Der Remoteserver hat einen Fehler zurückgegeben: (403) Verboten. ErrorDetails - unter C:\Program Files\WindowsPowerShell\Modules\MS Commerce\1.2\MS Commerce.psm1:216 char:5*<br>
*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Fehler beim Retri...*<br>
\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo : NotSpecified: (:) [Write-Error], WriteErrorException*<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*

Wenn Ihr Konto nicht über Die Rechte des Unternehmens- oder Abrechnungsadministrators verfügt, wenden Sie sich an Ihren IT-Administrator.
