---
title: Verwenden von DLP in Transportregeln
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 00ea5e67d1277e4a2a73d616b1f90d6e4bc5b54f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773162"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="61c89-102">Verwenden von DLP in Transportregeln</span><span class="sxs-lookup"><span data-stu-id="61c89-102">Using DLP in transport rules</span></span>

<span data-ttu-id="61c89-103">Wenn Sie die Verhinderung von Datenverlust (DLP) in einen vorhandenen Transport integrieren möchten, verwenden Sie die Bedingung "**Wenn die Nachricht enthält... Vertrauliche Informationen**" in der Einstellung der Transportregel.</span><span class="sxs-lookup"><span data-stu-id="61c89-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="61c89-104">**Weitere Informationen finden Sie hier:**</span><span class="sxs-lookup"><span data-stu-id="61c89-104">**For more details, see:**</span></span>

- <span data-ttu-id="61c89-105">Integrierte DLP-Typen vertraulicher Informationen in Transportregeln: [Integrieren von Regeln für vertrauliche Informationen](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="61c89-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="61c89-106">Sie können die Regel mit oder ohne Richtlinientest auch testen, indem Sie die Regel im Testmodus verwenden.</span><span class="sxs-lookup"><span data-stu-id="61c89-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="61c89-107">Sie sollten nach der Erstellung der Regel 30 Minuten warten, bevor Sie sie testen.</span><span class="sxs-lookup"><span data-stu-id="61c89-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="61c89-108">Siehe [Nachrichtenflussregel (Transportregel) testen](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules).</span><span class="sxs-lookup"><span data-stu-id="61c89-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="61c89-109">**Hinweis**: Wenn Sie eine neue DLP-Richtlinie mit Transportregeln im EAC implementieren möchten, verwenden Sie stattdessen [DLP-Richtlinien im Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="61c89-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
