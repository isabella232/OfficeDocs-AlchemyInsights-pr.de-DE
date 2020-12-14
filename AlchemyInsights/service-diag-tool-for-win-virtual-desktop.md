---
title: Dienst Diagnosetool für Windows Virtual Desktop
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/14/2020
ms.locfileid: "49665824"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Dienst Diagnosetool für Windows Virtual Desktop

Windows Virtual Desktop (Oktober) bietet ein Diagnosetool, mit dem Administratoren Fehler über eine einzelne Schnittstelle identifizieren können. Dieses Tool protokolliert Diagnose bezogene Informationen, wenn Oktober von einem Benutzer verwendet wird, dem eine Oktober-Rolle zugewiesen ist. Jedes Protokoll enthält Informationen über die an der Aktivität beteiligte Oktober-Rolle, die Fehlermeldungen, die während der Sitzung angezeigt werden, sowie Informationen über den Mandanten und den Benutzer. Azure Log Analytics kann so konfiguriert werden, dass das vom Diagnosetool erstellte Aktivitätsprotokoll erfasst wird. Dazu gehen Sie so vor:

1. Erstellen Sie einen Log Analytics-Arbeitsbereich mit dem [Azure-Portal](https://go.microsoft.com/fwlink/?linkid=2129500) oder [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Verbinden Sie Windows-Computer mit Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Rufen Sie die Arbeitsbereichs-ID und den Primärschlüssel Ihres Arbeitsbereichs ab. Der Setup-Assistent benötigt diese Informationen, um den Agent ordnungsgemäß zu konfigurieren und sicherzustellen, dass er mit Azure Monitor kommunizieren kann.
1. [Drücken Sie Diagnosedaten in den Arbeitsbereich](https://go.microsoft.com/fwlink/?linkid=2128284). Sie können Diagnosedaten von Ihrem Oktober-Mandanten in die Protokollanalyse für Ihren Arbeitsbereich verschieben.
1. [Identifizieren und diagnostizieren](https://go.microsoft.com/fwlink/?linkid=2128338) Sie interne oder externe Probleme im Zusammenhang mit Oktober.

Weitere Informationen zum Konfigurieren des Dienst Diagnosetools für Oktober finden Sie unter [use Log Analytics for the Diagnostics Feature](https://go.microsoft.com/fwlink/?linkid=2128084).
