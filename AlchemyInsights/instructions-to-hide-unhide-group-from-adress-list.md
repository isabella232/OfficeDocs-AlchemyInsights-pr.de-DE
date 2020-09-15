---
title: Anweisungen zum Ausblenden/Einblenden von Gruppen aus der Adressliste
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663008"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="40159-102">Ausblenden der Microsoft 365-Gruppe aus Adressliste (GAL)</span><span class="sxs-lookup"><span data-stu-id="40159-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="40159-103">Verwenden Sie den folgenden Befehl in der Exo-Shell, um eine Microsoft 365-Gruppe aus Adresslisten (GAL) von Exchange-Clients (wie Outlook oder OWA) auszublenden:</span><span class="sxs-lookup"><span data-stu-id="40159-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="40159-104">Verwenden Sie den folgenden Befehl in der Exo-Shell, um die Microsoft 365-Gruppe auszublenden und für Exchange-Clients sichtbar zu sein:</span><span class="sxs-lookup"><span data-stu-id="40159-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

