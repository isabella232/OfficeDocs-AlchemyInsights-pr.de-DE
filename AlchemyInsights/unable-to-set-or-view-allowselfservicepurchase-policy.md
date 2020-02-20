---
title: Die AllowSelfServicePurchase-Richtlinie kann nicht festgelegt oder angezeigt werden
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158560"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="cb2c9-102">Die AllowSelfServicePurchase-Richtlinie kann nicht festgelegt oder angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="cb2c9-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="cb2c9-103">Beim Versuch, die AllowSelfServicePurchase-Richtlinie festzulegen oder anzuzeigen, wird die folgende Fehlermeldung angezeigt:</span><span class="sxs-lookup"><span data-stu-id="cb2c9-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="cb2c9-104">*HandleError: Fehler beim Abrufen der Produktrichtlinie mit der Richtlinien-Nr "AllowSelfServicePurchase", ErrorMessage – die zugrunde liegende Verbindung wurde geschlossen: ein unerwarteter Fehler ist bei einem senden aufgetreten.*</span><span class="sxs-lookup"><span data-stu-id="cb2c9-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="cb2c9-105">Dies kann an einer älteren Version von Transport Layer Security (TLS) liegen.</span><span class="sxs-lookup"><span data-stu-id="cb2c9-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="cb2c9-106">Um den MSCommerce-Dienst zu verbinden, müssen Sie TLS 1,2 oder höher verwenden.</span><span class="sxs-lookup"><span data-stu-id="cb2c9-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="cb2c9-107">Führen Sie die folgenden Schritte aus, um das TLS-Protokoll auf 1,2, überprüfen und wiederholen zu aktivieren/festzulegen.</span><span class="sxs-lookup"><span data-stu-id="cb2c9-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="cb2c9-108">Geben Sie an der PowerShell-Eingabeaufforderung (\) PS C: den folgenden Befehl ein, um das TLS-Protokoll auf Version 1,2 festzulegen:</span><span class="sxs-lookup"><span data-stu-id="cb2c9-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="cb2c9-109">Überprüfen Sie mit dem folgenden Befehl die verwendeten TLS-Protokolle (n):</span><span class="sxs-lookup"><span data-stu-id="cb2c9-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="cb2c9-110">Wiederholen Sie die Befehle Get oder Update bei Bedarf.</span><span class="sxs-lookup"><span data-stu-id="cb2c9-110">Retry the Get or Update commands as needed.</span></span>

