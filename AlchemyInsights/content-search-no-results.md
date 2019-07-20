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
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800346"
---
# <a name="no-results-from-content-searchexports"></a>Keine Ergebnisse aus der Inhaltssuche/Exporte

Probleme bei der Inhaltssuche/Exporte, die keine Daten zurückgeben, können an einem bestimmten Compliance-Sicherheits Filter liegen, der von einem bestimmten Administrator eingerichtet wurde und nicht an alle Administratoren kommuniziert.

Um dies zu beheben, überprüfen Sie, ob es irgendwelche Compliance-Sicherheitsfilter gibt, die dies möglicherweise verursachen:
1. Herstellen einer Verbindung mit dem Security and Compliance Center PowerShell
2. Führen Sie den folgenden Cmdlets aus:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-Organization $org