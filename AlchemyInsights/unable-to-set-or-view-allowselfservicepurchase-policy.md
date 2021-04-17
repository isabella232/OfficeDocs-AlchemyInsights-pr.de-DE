---
title: Die AllowSelfServicePurchase-Richtlinie kann nicht festgelegt oder angezeigt werden.
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
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826090"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="56a92-102">Die AllowSelfServicePurchase-Richtlinie kann nicht festgelegt oder angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="56a92-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="56a92-103">Wenn Sie versuchen, die AllowSelfServicePurchase-Richtlinie zu festlegen oder anzeigen, wird die folgende Fehlermeldung angezeigt:</span><span class="sxs-lookup"><span data-stu-id="56a92-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="56a92-104">*HandleError : Fehler beim Abrufen der Produktrichtlinie mit PolicyId 'AllowSelfServicePurchase', ErrorMessage – Die zugrunde liegende Verbindung wurde geschlossen: Bei einem Senden ist ein unerwarteter Fehler aufgetreten.*</span><span class="sxs-lookup"><span data-stu-id="56a92-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="56a92-105">Dies liegt möglicherweise an einer älteren Version von Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="56a92-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="56a92-106">Zum Verbinden des MS Commerce-Diensts müssen Sie TLS 1.2 oder höher verwenden.</span><span class="sxs-lookup"><span data-stu-id="56a92-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="56a92-107">Führen Sie die folgenden Schritte aus, um das TLS-Protokoll auf 1.2 zu aktivieren bzw. auf 1.2 zu setzen, zu überprüfen und erneut zu versuchen.</span><span class="sxs-lookup"><span data-stu-id="56a92-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="56a92-108">Geben Sie an der #A0 (PS C: geben Sie den folgenden Befehl ein, um das \) #A1 auf Version 1.2 zu setzen:</span><span class="sxs-lookup"><span data-stu-id="56a92-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="56a92-109">Überprüfen Sie die verwendeten TLS-Protokolle mit dem folgenden Befehl:</span><span class="sxs-lookup"><span data-stu-id="56a92-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="56a92-110">Wiederholen Sie die Befehle Get oder Update nach Bedarf.</span><span class="sxs-lookup"><span data-stu-id="56a92-110">Retry the Get or Update commands as needed.</span></span>

