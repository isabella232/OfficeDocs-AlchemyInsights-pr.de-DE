---
title: Ausgehender Relaypool
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/08/2021
ms.locfileid: "53339965"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="efe3d-102">Ausgehender Relaypool</span><span class="sxs-lookup"><span data-stu-id="efe3d-102">Outbound relay pool</span></span>

<span data-ttu-id="efe3d-103">Microsoft unternimmt einige Änderungen an der Konfiguration für das Weiterleiten oder Weiterleiten von E-Mails über Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="efe3d-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="efe3d-104">Nachrichten in bestimmten Szenarien werden über Microsoft 365 mithilfe eines speziellen Relaypools weitergeleitet oder weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="efe3d-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="efe3d-105">Nachrichten, die mithilfe des Relaypools gesendet werden, können im Junk-E-Mail-Ordner des Empfängers enden.</span><span class="sxs-lookup"><span data-stu-id="efe3d-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="efe3d-106">Weitere Informationen finden Sie unter "Pools für [ausgehende Übermittlungen"](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="efe3d-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="efe3d-107">Um ein Szenario mithilfe des Relaypools zu vermeiden, stellen Sie sicher, dass weitergeleitete/weitergeleitete Nachrichten eines der folgenden Kriterien erfüllen:</span><span class="sxs-lookup"><span data-stu-id="efe3d-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="efe3d-108">Der ausgehende Absender ist eine akzeptierte Domäne des Mandanten.</span><span class="sxs-lookup"><span data-stu-id="efe3d-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="efe3d-109">Sender Policy Framework (SPF) wird übergeben, wenn die Nachricht an Microsoft 365 kommt.</span><span class="sxs-lookup"><span data-stu-id="efe3d-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="efe3d-110">DomainKeys Identified Mail (DKIM) in der P2-Absenderdomäne wird übergeben, wenn die Nachricht zu Microsoft 365 kommt.</span><span class="sxs-lookup"><span data-stu-id="efe3d-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="efe3d-111">Nachrichten, die die oben genannten Kriterien erfüllen, werden nicht über den Relaypool weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="efe3d-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="efe3d-112">Wenn der MX-Eintrag für Ihre Domäne auf einen Drittanbieterserver oder einen lokalen Server verweist, verwenden Sie erweiterte Filterung, um sicherzustellen, dass die SPF-Überprüfung für eingehende E-Mails korrekt ist, und um das Senden von E-Mails über den Relaypool zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="efe3d-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="efe3d-113">**Wie können wir feststellen, ob wir vom Relaypool betroffen sind?**</span><span class="sxs-lookup"><span data-stu-id="efe3d-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="efe3d-114">Wenn Ihre weitergeleiteten oder weitergeleiteten E-Mails eines der oben genannten Kriterien verwenden, werden Nachrichten nicht über den Relaypool weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="efe3d-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="efe3d-115">Wenn eine Nachricht jedoch über einen Relaypool gesendet wird, befindet sich die ip-Adresse des ausgehenden Servers im Bereich 40.95.0.0/16, und der Name des ausgehenden Servers enthält **den** Namen.</span><span class="sxs-lookup"><span data-stu-id="efe3d-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

