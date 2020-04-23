---
title: Problembehandlung des Sicherheitstipps für die Überprüfung der Betrugserkennung
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 61159391f7a9876750cd7fefc40c54054fb9bec9
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759511"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="ea805-102">Problembehandlung des Sicherheitstipps für die Überprüfung der Betrugserkennung</span><span class="sxs-lookup"><span data-stu-id="ea805-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="ea805-103">Wenn Sie einen Sicherheitstipp erhalten, der besagt, dass der Absender unsere Betrugs Erkennungs Prüfungen nicht ausgeführt hat und möglicherweise nicht angezeigt wird, konnte der Absender weder DKIM-noch SPF-Authentifizierungsprüfungen übergeben.</span><span class="sxs-lookup"><span data-stu-id="ea805-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="ea805-104">Die beste Methode zum Beheben dieses Problem liegt darin, dass sich der Absender selbst autorisieren kann.</span><span class="sxs-lookup"><span data-stu-id="ea805-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="ea805-105">Wenn der Absender in Ihrem Auftrag sendet, müssen Sie ihn autorisieren, indem Sie die IP-Adresse des Absenders zu Ihrem SPF-Eintrag hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="ea805-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="ea805-106">Weitere Informationen finden Sie unter [Problembehandlung des roten (verdächtigen) Sicherheitstipps für die Betrugs Erkennungs Überprüfung](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="ea805-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="ea805-107">Hier sind einige weitere Links, die helfen können:</span><span class="sxs-lookup"><span data-stu-id="ea805-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="ea805-108">Verwenden von SPF (Sender Policy Framework) zur Verhinderung von Spoofing durch Microsoft</span><span class="sxs-lookup"><span data-stu-id="ea805-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="ea805-109">Einrichten von SPF zum Verhindern von Spoofing</span><span class="sxs-lookup"><span data-stu-id="ea805-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
