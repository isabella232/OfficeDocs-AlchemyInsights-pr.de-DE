---
title: Problembehandlung beim Sicherheitstipp für Betrugs Erkennungs Prüfungen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 98627edcd2b685673dda8a8a18821eddf9b64bc1
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391208"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="68907-102">Problembehandlung beim Sicherheitstipp für Betrugs Erkennungs Prüfungen</span><span class="sxs-lookup"><span data-stu-id="68907-102">Troubleshooting the safety tip for fraud detection checks</span></span>



<span data-ttu-id="68907-103">Wenn Sie einen Sicherheitstipp erhalten, der besagt, dass der Absender unsere Betrugserkennung nicht überprüft und möglicherweise nicht angezeigt hat, kann der Absender weder DKIM-noch SPF-Authentifizierungsüberprüfungen durchführen.</span><span class="sxs-lookup"><span data-stu-id="68907-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="68907-104">Die beste Methode, um dies zu beheben, besteht darin, dass der Absender sich selbst autorisiert.</span><span class="sxs-lookup"><span data-stu-id="68907-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="68907-105">Wenn der Absender in Ihrem Namen sendet, müssen Sie ihn autorisieren, indem Sie die IP-Adresse des Absenders zu Ihrem SPF-Eintrag hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="68907-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="68907-106">Weitere Informationen finden Sie unter [Troubleshooting the Red (suspekt) Safety Tip for Betrugs Detection Checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="68907-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="68907-107">Hier einige weitere Links, die Ihnen helfen können:</span><span class="sxs-lookup"><span data-stu-id="68907-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="68907-108">Wie Office 365 das SPF (Sender Policy Framework) verwendet, um Spoofing zu verhindern</span><span class="sxs-lookup"><span data-stu-id="68907-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="68907-109">Einrichten von SPF in Office 365 zum Verhindern von Spoofing</span><span class="sxs-lookup"><span data-stu-id="68907-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

