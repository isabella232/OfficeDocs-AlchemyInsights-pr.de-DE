---
title: Beheben von Transportregeln
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568559"
---
# <a name="fix-transport-rules"></a>Beheben von Transportregeln

Diese Nachricht wurde von einer benutzerdefinierten Nachrichtenflussregel beeinflusst. Gehen Sie wie folgt vor, um die genaue Regel zu überprüfen:

1. Notieren Sie sich in den Übermittlungsergebnissen unter **Zusätzliche Informationen** die **GUID** oder **den Richtliniennamen**.
2. Starten Sie die Exchange-Verwaltungsshell. Weitere Informationen finden Sie unter [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Führen Sie diesen Befehl aus (mithilfe der GUID aus Ihrer Übermittlung):  **Get-TransportRule -identity "GUID" | fl * Description***
4. Überprüfen Sie die Beschreibung, um die konfigurierten Bedingungen zu sehen, die sich auf die Nachricht ausdrückten.

Weitere Informationen finden Sie unter [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
