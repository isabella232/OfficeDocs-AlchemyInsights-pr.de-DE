---
title: Problembehandlung des Sicherheitstipps für die Überprüfung der Betrugserkennung
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
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 7ce8bcc7caefebf51fc8d9622367fd16405deef1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533180"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="8fa66-102">Problembehandlung des Sicherheitstipps für die Überprüfung der Betrugserkennung</span><span class="sxs-lookup"><span data-stu-id="8fa66-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="8fa66-103">Wenn Sie einen Sicherheitstipp erhalten, der besagt, dass der Absender unsere Betrugs Erkennungs Prüfungen nicht ausgeführt hat und möglicherweise nicht angezeigt wird, konnte der Absender weder DKIM-noch SPF-Authentifizierungsprüfungen übergeben.</span><span class="sxs-lookup"><span data-stu-id="8fa66-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="8fa66-104">Die beste Methode zum Beheben dieses Problem liegt darin, dass sich der Absender selbst autorisieren kann.</span><span class="sxs-lookup"><span data-stu-id="8fa66-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="8fa66-105">Wenn der Absender in Ihrem Auftrag sendet, müssen Sie ihn autorisieren, indem Sie die IP-Adresse des Absenders zu Ihrem SPF-Eintrag hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="8fa66-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="8fa66-106">Weitere Informationen finden Sie unter [Problembehandlung des roten (verdächtigen) Sicherheitstipps für die Betrugs Erkennungs Überprüfung](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="8fa66-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="8fa66-107">Hier sind einige weitere Links, die helfen können:</span><span class="sxs-lookup"><span data-stu-id="8fa66-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="8fa66-108">Verwenden von SPF (Sender Policy Framework) zur Verhinderung von Spoofing durch Office 365</span><span class="sxs-lookup"><span data-stu-id="8fa66-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="8fa66-109">Einrichten von SPF in Office 365 zum Verhindern von Spoofing</span><span class="sxs-lookup"><span data-stu-id="8fa66-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
