---
title: Während der Inhaltssuche/des Exports werden keine Ergebnisse zurückgegeben.
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/14/2020
ms.locfileid: "49666650"
---
# <a name="no-results-returned-during-content-searchexport"></a>Während der Inhaltssuche/des Exports werden keine Ergebnisse zurückgegeben.

Wenn Probleme mit den folgenden eDiscovery-Szenarien auftreten:

- Inhaltssuche/-Export gibt keine Daten oder unerwartete Daten zurück
- eDiscovery-Suche oder-Export schlägt fehl

Dies kann auf bestimmte Compliance-Sicherheitsfilter zurückzuführen sein, die von einem bestimmten Administrator eingerichtet wurden und nicht allen Administratoren mitgeteilt wurden.

Um dies zu beheben, überprüfen Sie, ob es irgendwelche Compliance-Sicherheitsfilter gibt, die diese Probleme verursachen könnten:

1. Herstellen einer Verbindung mit dem Security and Compliance Center PowerShell
2. Führen Sie den folgenden Cmdlets aus:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Weitere Informationen zu Compliance-Sicherheitsfiltern finden Sie unter [Berechtigungs Filterung für die Inhaltssuche](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
