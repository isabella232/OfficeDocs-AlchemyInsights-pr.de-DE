---
title: Inhaltssuche Keine Ergebnisse
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816847"
---
# <a name="no-results-from-content-searchexports"></a>Keine Ergebnisse aus inhaltssuche/export

Probleme mit der Inhaltssuche/-exporten, die keine Daten zurückgeben, können auf bestimmten Compliancesicherheitsfilter zurück, der von einem bestimmten Administrator eingerichtet wurde und nicht an alle Administratoren kommuniziert wurde.

Um dies zu beheben, überprüfen Sie, ob Kompatibilitätssicherheitsfilter enthalten sind, die dies verursachen können:
1. Herstellen einer Verbindung mit Security and Compliance Center Powershell
2. Führen Sie die folgenden Befehlslets aus:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org