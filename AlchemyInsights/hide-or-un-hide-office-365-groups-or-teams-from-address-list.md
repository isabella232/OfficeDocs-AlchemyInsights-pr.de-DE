---
title: Office 365-Gruppen oder -Teams auf der Adressliste aus- oder einblenden
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: cb3c2819ff7203774511bd0e45633b59a02091ff
ms.sourcegitcommit: e3a1f96200bc58dc8a5b3597cc2600e71c4bd266
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/14/2020
ms.locfileid: "44225378"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a><span data-ttu-id="61d2e-102">Office 365-Gruppen oder -Teams auf der Adressliste aus- oder einblenden</span><span class="sxs-lookup"><span data-stu-id="61d2e-102">Hide or un-hide Office 365 groups or teams from address list</span></span>

<span data-ttu-id="61d2e-103">Verwenden Sie den folgenden EXO PowerShell-Befehl, um Office 365-Gruppen/-Teams auf Adresslisten (Globale Adressliste, GAL) von Exchange-Clients (Outlook, OWA) aus- oder einzublenden:</span><span class="sxs-lookup"><span data-stu-id="61d2e-103">Use the following EXO PowerShell command to hide or un-hide Office 365 group/teams from address lists (GAL) of Exchange clients (Outlook, OWA):</span></span>

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

<span data-ttu-id="61d2e-104">Verwenden Sie den folgenden EXO PowerShell-Befehl, um die Office 365-Gruppen/-Teams von Exchange-Clients (Outlook, OWA) aus oder einzublenden:</span><span class="sxs-lookup"><span data-stu-id="61d2e-104">Use the following EXO PowerShell command to hide or un-hide the Office365 group/teams from Exchange clients (Outlook, OWA):</span></span>

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- <span data-ttu-id="61d2e-105">Detaillierte Anweisungen finden Sie unter [Ausblenden von Office 365-Gruppen auf der GAL und Exchange-Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span><span class="sxs-lookup"><span data-stu-id="61d2e-105">For detailed instructions, see [Hide Office 365 Groups from the GAL and Exchange Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span></span>
