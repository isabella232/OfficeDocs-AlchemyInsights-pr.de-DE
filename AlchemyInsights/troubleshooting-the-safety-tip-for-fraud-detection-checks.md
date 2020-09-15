---
title: Problembehandlung des Sicherheitstipps für die Überprüfung der Betrugserkennung
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658409"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Problembehandlung des Sicherheitstipps für die Überprüfung der Betrugserkennung

Wenn Sie einen Sicherheitstipp erhalten, der besagt, dass der Absender unsere Betrugs Erkennungs Prüfungen nicht ausgeführt hat und möglicherweise nicht angezeigt wird, konnte der Absender weder DKIM-noch SPF-Authentifizierungsprüfungen übergeben. Die beste Methode zum Beheben dieses Problem liegt darin, dass sich der Absender selbst autorisieren kann. Wenn der Absender in Ihrem Auftrag sendet, müssen Sie ihn autorisieren, indem Sie die IP-Adresse des Absenders zu Ihrem SPF-Eintrag hinzufügen.
  
Weitere Informationen finden Sie unter [Problembehandlung des roten (verdächtigen) Sicherheitstipps für die Betrugs Erkennungs Überprüfung](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .
  
Hier sind einige weitere Links, die helfen können:
  
- [Verwenden von SPF (Sender Policy Framework) zur Verhinderung von Spoofing durch Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Einrichten von SPF zum Verhindern von Spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
