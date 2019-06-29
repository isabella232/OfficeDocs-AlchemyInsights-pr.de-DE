---
title: 1332 OWA-Postfachregel (n) werden nicht für ein Postfach ausgeführt
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 7d1848830847fc6722da20e09a4875f49bf02bd3
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35360916"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Eine Posteingangsregel funktioniert nicht wie erwartet

Überprüfen Sie die folgenden Einstellungen:

- Eine Nachricht kann nur einmal automatisch basierend auf Posteingangsregeln umgeleitet, weitergeleitet oder beantwortet werden. Eine Umleitungsregel (eine Posteingangsregel oder eine Nachrichtenfluss Regel, die auch als Transportregel bezeichnet wird) kann maximal zehn Weiterleitungs Empfänger zu einer Nachricht hinzufügen. Weitere Informationen finden Sie unter [Journal-, Transport-und Posteingangsregel Grenzwerte](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Posteingangsregeln funktionieren nicht mit dem alternativen Journalpostfach. Weitere Informationen zum alternativen Journalpostfach finden Sie unter [alternative Journalpostfach](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Um diese Probleme zu beheben, lesen Sie [KB 2829319](https://support.microsoft.com/kb/2829319).

Wenn die vorherigen Probleme nicht zutreffen, führen Sie den Diagnosebericht "Posteingangsregel" aus, bevor Sie das Problem an den Microsoft-Support eskalieren:

1. Öffnen Sie das Postfach in Outlook im Internet, und klicken Sie auf **Einstellungen** \> **Optionen** \> **e-Mail-** \> **Posteingangsregeln**organisieren.

2. Klicken Sie unten auf der Seite auf **Wenn Ihre Regeln nicht funktionieren klicken Sie hier, um einen Diagnosebericht zu erstellen**.
