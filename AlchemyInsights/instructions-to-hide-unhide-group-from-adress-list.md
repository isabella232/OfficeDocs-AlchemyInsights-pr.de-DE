---
title: Anweisungen zum Ausblenden/Einblenden von Gruppen aus der Adressliste
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908343"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="13089-102">Ausblenden der Microsoft 365-Gruppe aus Adressliste (GAL)</span><span class="sxs-lookup"><span data-stu-id="13089-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="13089-103">Um eine Microsoft 365-Gruppe aus Adresslisten (GAL) von Exchange-Clients (wie Outlook oder OWA) auszublenden, verwenden Sie den folgenden Befehl in Exo Shell:</span><span class="sxs-lookup"><span data-stu-id="13089-103">To hide an Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="13089-104">Verwenden Sie den folgenden Befehl in der Exo-Shell, um die Microsoft 365-Gruppe auszublenden und für Exchange-Clients sichtbar zu sein:</span><span class="sxs-lookup"><span data-stu-id="13089-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

