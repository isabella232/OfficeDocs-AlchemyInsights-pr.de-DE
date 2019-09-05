---
title: Aktivieren der Postfachüberwachung
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736252"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="29f6e-102">Aktivieren der Postfachüberwachung</span><span class="sxs-lookup"><span data-stu-id="29f6e-102">Enable mailbox auditing</span></span>

<span data-ttu-id="29f6e-103">Um die postfachüberwachung für einen einzelnen Benutzer oder eine gesamte Organisation zu aktivieren, müssen die folgenden Cmdlets von der Remote-Power Shell aus ausgeführt werden:</span><span class="sxs-lookup"><span data-stu-id="29f6e-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="29f6e-104">**Einzelner Benutzer**</span><span class="sxs-lookup"><span data-stu-id="29f6e-104">**Single User**</span></span>
  
<span data-ttu-id="29f6e-105">Festlegen-Mailbox-Identity "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="29f6e-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="29f6e-106">**Organisation**</span><span class="sxs-lookup"><span data-stu-id="29f6e-106">**Organization**</span></span>
  
<span data-ttu-id="29f6e-107">Get-Mailbox-resultse Unlimited-Filter {RecipientTypeDetails-EQ "User Mailbox"} | Festlegen-Mailbox-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="29f6e-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="29f6e-108">Weitere Informationen</span><span class="sxs-lookup"><span data-stu-id="29f6e-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

