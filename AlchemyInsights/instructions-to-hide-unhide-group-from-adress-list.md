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
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Ausblenden der Microsoft 365-Gruppe aus Adressliste (GAL)

Verwenden Sie den folgenden Befehl in der Exo-Shell, um eine Microsoft 365-Gruppe aus Adresslisten (GAL) von Exchange-Clients (wie Outlook oder OWA) auszublenden:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Verwenden Sie den folgenden Befehl in der Exo-Shell, um die Microsoft 365-Gruppe auszublenden und für Exchange-Clients sichtbar zu sein:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

