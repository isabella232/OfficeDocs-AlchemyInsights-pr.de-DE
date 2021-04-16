---
title: Office 365-Gruppen oder -Teams auf der Adressliste aus- oder einblenden
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811455"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a><span data-ttu-id="6334b-102">Office 365-Gruppen oder -Teams auf der Adressliste aus- oder einblenden</span><span class="sxs-lookup"><span data-stu-id="6334b-102">Hide or un-hide Office 365 groups or teams from address list</span></span>

<span data-ttu-id="6334b-103">Verwenden Sie den folgenden EXO PowerShell-Befehl, um Office 365-Gruppen/-Teams auf Adresslisten (Globale Adressliste, GAL) von Exchange-Clients (Outlook, OWA) aus- oder einzublenden:</span><span class="sxs-lookup"><span data-stu-id="6334b-103">Use the following EXO PowerShell command to hide or un-hide Office 365 group/teams from address lists (GAL) of Exchange clients (Outlook, OWA):</span></span>

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

<span data-ttu-id="6334b-104">Verwenden Sie den folgenden EXO PowerShell-Befehl, um die Office 365-Gruppen/-Teams von Exchange-Clients (Outlook, OWA) aus oder einzublenden:</span><span class="sxs-lookup"><span data-stu-id="6334b-104">Use the following EXO PowerShell command to hide or un-hide the Office365 group/teams from Exchange clients (Outlook, OWA):</span></span>

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- <span data-ttu-id="6334b-105">Detaillierte Anweisungen finden Sie unter [Ausblenden von Office 365-Gruppen auf der GAL und Exchange-Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span><span class="sxs-lookup"><span data-stu-id="6334b-105">For detailed instructions, see [Hide Office 365 Groups from the GAL and Exchange Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span></span>
