---
title: Inhaltssuche keine Ergebnisse
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680646"
---
# <a name="no-results-from-content-searchexports"></a>Keine Ergebnisse aus der Inhaltssuche/Exporte

Probleme bei der Inhaltssuche/Exporte, die keine Daten zurückgeben, können an einem bestimmten Compliance-Sicherheits Filter liegen, der von einem bestimmten Administrator eingerichtet wurde und nicht an alle Administratoren kommuniziert.

Um dies zu beheben, überprüfen Sie, ob es irgendwelche Compliance-Sicherheitsfilter gibt, die dies möglicherweise verursachen:
1. Herstellen einer Verbindung mit dem Security and Compliance Center PowerShell
2. Führen Sie den folgenden Cmdlets aus:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-Organization $org