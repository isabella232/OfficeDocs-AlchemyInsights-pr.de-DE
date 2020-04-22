---
title: Fehler beim Senden von e-Mails, die von Spamhaus blockiert wurden
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714257"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="d8f8a-102">Fehler beim Senden von e-Mail: Client Host blockiert mit Spamhaus</span><span class="sxs-lookup"><span data-stu-id="d8f8a-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="d8f8a-103">Die IP-Adresse, die die Nachricht gesendet hat, befindet sich in einer Sperrliste im Besitz von [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="d8f8a-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="d8f8a-104">Gründe für die Blockierung durch Spamhaus sind kompromittierte Konten, gefährdete Computer, die eine öffentliche IP-Adresse teilen, und Richtlinien für Internetdienstanbieter (ISP).</span><span class="sxs-lookup"><span data-stu-id="d8f8a-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="d8f8a-105">Mögliche Korrekturen sind:</span><span class="sxs-lookup"><span data-stu-id="d8f8a-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="d8f8a-106">Bei blockierten eingehenden Nachrichten, bei denen Sie den Quell-e-Mail-Server steuern, müssen Sie die Ursache ermitteln und den Block von der Spamhaus-Website entfernen.</span><span class="sxs-lookup"><span data-stu-id="d8f8a-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="d8f8a-107">Bei blockierten eingehenden Nachrichten, bei denen die Quell-IP-Adresse einer anderen Person gehört, muss der Adress Besitzer den Block von der Spamhaus-Website entfernen.</span><span class="sxs-lookup"><span data-stu-id="d8f8a-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="d8f8a-108">Wenn sich die IP-Adresse in der Richtlinien Sperrliste befindet (PBL), kann der Besitzer eine andere statische IP-Adresse zuweisen oder die Adresse aus dem PBL entfernen.</span><span class="sxs-lookup"><span data-stu-id="d8f8a-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="d8f8a-109">Bei blockierten ausgehenden Nachrichten von ihrer mit Microsoft verbundenen Domäne können Sie diesen Fehler erhalten, wenn die Nachrichten über einen Drittanbieterdienst weitergeleitet werden.</span><span class="sxs-lookup"><span data-stu-id="d8f8a-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="d8f8a-110">Sie können ein Whois-Nachschlage Tool verwenden, um den Besitzer blockierter IP-Adressen zu finden.</span><span class="sxs-lookup"><span data-stu-id="d8f8a-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
