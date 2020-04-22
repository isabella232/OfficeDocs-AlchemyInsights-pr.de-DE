---
title: Aktivieren der Postfachüberwachung
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703570"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="1e1c0-102">Aktivieren der Postfachüberwachung</span><span class="sxs-lookup"><span data-stu-id="1e1c0-102">Enable mailbox auditing</span></span>

<span data-ttu-id="1e1c0-103">Um die postfachüberwachung für einen einzelnen Benutzer oder eine gesamte Organisation zu aktivieren, müssen die folgenden Cmdlets von der Remote-Power Shell aus ausgeführt werden:</span><span class="sxs-lookup"><span data-stu-id="1e1c0-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="1e1c0-104">**Einzelner Benutzer**</span><span class="sxs-lookup"><span data-stu-id="1e1c0-104">**Single User**</span></span>
  
<span data-ttu-id="1e1c0-105">Festlegen-Mailbox-Identity "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="1e1c0-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="1e1c0-106">**Organisation**</span><span class="sxs-lookup"><span data-stu-id="1e1c0-106">**Organization**</span></span>
  
<span data-ttu-id="1e1c0-107">Get-Mailbox-resultse Unlimited-Filter {RecipientTypeDetails-EQ "User Mailbox"} | Festlegen-Mailbox-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="1e1c0-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="1e1c0-108">Weitere Informationen</span><span class="sxs-lookup"><span data-stu-id="1e1c0-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

