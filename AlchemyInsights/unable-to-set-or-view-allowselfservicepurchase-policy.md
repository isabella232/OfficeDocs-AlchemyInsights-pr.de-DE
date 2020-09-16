---
title: Die AllowSelfServicePurchase-Richtlinie kann nicht festgelegt oder angezeigt werden
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
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735198"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="c9d8c-102">Die AllowSelfServicePurchase-Richtlinie kann nicht festgelegt oder angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="c9d8c-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="c9d8c-103">Beim Versuch, die AllowSelfServicePurchase-Richtlinie festzulegen oder anzuzeigen, wird die folgende Fehlermeldung angezeigt:</span><span class="sxs-lookup"><span data-stu-id="c9d8c-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="c9d8c-104">*HandleError: Fehler beim Abrufen der Produktrichtlinie mit der Richtlinien-Nr "AllowSelfServicePurchase", ErrorMessage – die zugrunde liegende Verbindung wurde geschlossen: ein unerwarteter Fehler ist bei einem senden aufgetreten.*</span><span class="sxs-lookup"><span data-stu-id="c9d8c-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="c9d8c-105">Dies kann an einer älteren Version von Transport Layer Security (TLS) liegen.</span><span class="sxs-lookup"><span data-stu-id="c9d8c-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="c9d8c-106">Um den MSCommerce-Dienst zu verbinden, müssen Sie TLS 1,2 oder höher verwenden.</span><span class="sxs-lookup"><span data-stu-id="c9d8c-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="c9d8c-107">Führen Sie die folgenden Schritte aus, um das TLS-Protokoll auf 1,2, überprüfen und wiederholen zu aktivieren/festzulegen.</span><span class="sxs-lookup"><span data-stu-id="c9d8c-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="c9d8c-108">Geben Sie an der PowerShell-Eingabeaufforderung (PS C: \) den folgenden Befehl ein, um das TLS-Protokoll auf Version 1,2 festzulegen:</span><span class="sxs-lookup"><span data-stu-id="c9d8c-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="c9d8c-109">Überprüfen Sie mit dem folgenden Befehl die verwendeten TLS-Protokolle (n):</span><span class="sxs-lookup"><span data-stu-id="c9d8c-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="c9d8c-110">Wiederholen Sie die Befehle Get oder Update bei Bedarf.</span><span class="sxs-lookup"><span data-stu-id="c9d8c-110">Retry the Get or Update commands as needed.</span></span>

