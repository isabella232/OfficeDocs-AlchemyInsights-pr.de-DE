---
title: Fehler beim Senden von e-Mails, die von SpamHaus blockiert wurden
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 7d6ad2667613ae948a4abcefafe8d91cf89d2418
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/22/2019
ms.locfileid: "30761632"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="eb73b-102">Fehler beim Senden von e-Mails: Client Host mit Spamhaus blockiert</span><span class="sxs-lookup"><span data-stu-id="eb73b-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="eb73b-103">Die IP-Adresse, die die Nachricht gesendet hat, befindet sich in einer Sperrliste von [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="eb73b-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="eb73b-104">Gründe für die Blockierung durch Spamhaus sind kompromittierte Konten, kompromittierte Computer mit einer öffentlichen IP-Adresse und InternetdienstAnbieter-Richtlinien.</span><span class="sxs-lookup"><span data-stu-id="eb73b-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="eb73b-105">Mögliche Korrekturen sind:</span><span class="sxs-lookup"><span data-stu-id="eb73b-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="eb73b-106">Für blockierte eingehende Nachrichten an Office 365, bei denen Sie den Quell-e-Mail-Server steuern, müssen Sie die Ursache ermitteln und den Block aus der Spamhaus-Website entfernen.</span><span class="sxs-lookup"><span data-stu-id="eb73b-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="eb73b-107">Für blockierte eingehende Nachrichten an Office 365, bei denen die Quell-IP-Adresse zu einer anderen Person gehört, muss der Adress Besitzer den Block von der Spamhaus-Website entfernen.</span><span class="sxs-lookup"><span data-stu-id="eb73b-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="eb73b-108">Wenn sich die IP-Adresse in der Richtlinien Sperrliste (PBL) befindet, kann der Besitzer eine andere statische IP-Adresse zuweisen oder die Adresse aus dem PBL entfernen.</span><span class="sxs-lookup"><span data-stu-id="eb73b-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="eb73b-109">Für blockierte ausgehende Nachrichten von Ihrer Office 365-Domäne können Sie diese Fehlermeldung erhalten, wenn die Nachrichten über einen Drittanbieterdienst weitergeleitet werden.</span><span class="sxs-lookup"><span data-stu-id="eb73b-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="eb73b-110">Sie können ein WHOIS-Nachschlage Tool verwenden, um den blockierten IP-Adress Besitzer zu finden.</span><span class="sxs-lookup"><span data-stu-id="eb73b-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    

