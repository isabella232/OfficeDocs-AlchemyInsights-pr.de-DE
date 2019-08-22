---
title: Inhaltssuche keine Ergebnisse
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516778"
---
# <a name="no-results-from-content-searchexports"></a>Keine Ergebnisse aus der Inhaltssuche/Exporte

Probleme bei der Inhaltssuche/Exporte, die keine Daten zurückgeben, können an einem bestimmten Compliance-Sicherheits Filter liegen, der von einem bestimmten Administrator eingerichtet wurde und nicht an alle Administratoren kommuniziert.

Um dies zu beheben, überprüfen Sie, ob es irgendwelche Compliance-Sicherheitsfilter gibt, die dies möglicherweise verursachen:
1. Herstellen einer Verbindung mit dem Security and Compliance Center PowerShell
2. Führen Sie den folgenden Cmdlets aus:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-Organization $org