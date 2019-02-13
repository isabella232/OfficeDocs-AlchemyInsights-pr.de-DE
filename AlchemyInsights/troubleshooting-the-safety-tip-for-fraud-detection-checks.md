---
title: Überprüft die Sicherheit Tipps für die Erkennung von Betrug zur Problembehandlung
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
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29936359"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="78913-102">Überprüft die Sicherheit Tipps für die Erkennung von Betrug zur Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="78913-102">Troubleshooting the safety tip for fraud detection checks</span></span>



<span data-ttu-id="78913-p101">Wenn Sie sind einem Tipp Safety abrufen, die besagt, dass "Absender Fehler bei unseren Betrug Erkennung überprüft und möglicherweise nicht, die sie zu sein scheinen" und dann der Absender konnte nicht Prüfung auf DKIM oder SPF-Authentifizierung erfolgreich. Die beste Methode zur Lösung des Problems ist für den Absender zum Autorisieren von sich selbst. Wenn der Absender in Ihrem Auftrag sendet, müssen Sie sie autorisieren, indem Sie die IP-Adresse des Absenders SPF-Datensatz hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="78913-p101">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks. The best method to resolve this is for the sender to authorize themselves. If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="78913-106">Weitere Informationen finden Sie unter [Problembehandlung Rot (verdächtigen) Safety Tipp für Betrug Erkennung überprüft](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="78913-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="78913-107">Hier sind einige andere Links, die helfen:</span><span class="sxs-lookup"><span data-stu-id="78913-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="78913-108">Wie Office 365 Sender Policy Framework (SPF) verwendet, um zu verhindern, dass spoofing</span><span class="sxs-lookup"><span data-stu-id="78913-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="78913-109">Einrichten von SPF in Office 365 zum Verhindern von Spoofing</span><span class="sxs-lookup"><span data-stu-id="78913-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

