---
title: Problembehandlung beim Sicherheitstipp für Betrugserkennungsüberprüfungen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834730"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Problembehandlung beim Sicherheitstipp für Betrugserkennungsüberprüfungen

Wenn Sie einen Sicherheitstipp erhalten, der "Der Absender hat unsere Betrugserkennungsüberprüfungen nicht bestanden und möglicherweise nicht der Absender ist, um den es sich handelt", hat der Absender keine DKIM- oder SPF-Authentifizierungsüberprüfungen bestanden. Die beste Methode, um dies zu beheben, ist, dass sich der Absender selbst autorisiert. Wenn der Absender in Ihrem Namen sendet, müssen Sie sie autorisieren, indem Sie die IP-Adresse des Absenders zu Ihrem SPF-Eintrag hinzufügen.
  
Weitere [Informationen finden Sie unter Troubleshooting the red (suspicious) safety tip for fraud detection](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) checks.
  
Hier sind einige weitere Links, die Ihnen helfen können:
  
- [So verwendet Microsoft das Sender Policy Framework (SPF), um Spoofing zu verhindern](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Einrichten von SPF zum Verhindern von Spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
