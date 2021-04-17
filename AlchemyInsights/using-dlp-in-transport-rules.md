---
title: Verwenden von DLP in Transportregeln
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827215"
---
# <a name="using-dlp-in-transport-rules"></a>Verwenden von DLP in Transportregeln

Wenn Sie die Verhinderung von Datenverlust (DLP) in einen vorhandenen Transport integrieren möchten, verwenden Sie die Bedingung "**Wenn die Nachricht enthält... Vertrauliche Informationen**" in der Einstellung der Transportregel.

**Weitere Informationen finden Sie hier:**

- Integrierte DLP-Typen vertraulicher Informationen in Transportregeln: [Integrieren von Regeln für vertrauliche Informationen](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).

Sie können die Regel mit oder ohne Richtlinientest auch testen, indem Sie die Regel im Testmodus verwenden.  Sie sollten nach der Erstellung der Regel 30 Minuten warten, bevor Sie sie testen.

- Siehe [Nachrichtenflussregel (Transportregel) testen](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules).

**Hinweis**: Wenn Sie eine neue DLP-Richtlinie mit Transportregeln im EAC implementieren möchten, verwenden Sie stattdessen [DLP-Richtlinien im Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).
