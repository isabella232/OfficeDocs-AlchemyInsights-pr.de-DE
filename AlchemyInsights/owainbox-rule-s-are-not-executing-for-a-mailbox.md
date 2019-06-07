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
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 28b03183552e00dd2522fff51b061cc27d5032ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762222"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Eine Posteingangsregel funktioniert nicht wie erwartet

Überprüfen Sie die folgenden Einstellungen:

- Eine Nachricht kann nur einmal automatisch basierend auf Posteingangsregeln umgeleitet, weitergeleitet oder beantwortet werden. Eine Umleitungsregel (eine Posteingangsregel oder eine Nachrichtenfluss Regel, die auch als Transportregel bezeichnet wird) kann maximal zehn Weiterleitungs Empfänger zu einer Nachricht hinzufügen. Weitere Informationen finden Sie unter [Journal-, Transport-und Posteingangsregel Grenzwerte](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Posteingangsregeln funktionieren nicht mit dem alternativen Journalpostfach. Weitere Informationen zum alternativen Journalpostfach finden Sie unter [alternative Journalpostfach](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Um diese Probleme zu beheben, lesen Sie [KB 2829319](https://support.microsoft.com/kb/2829319).

Wenn die vorherigen Probleme nicht zutreffen, führen Sie den Diagnosebericht "Posteingangsregel" aus, bevor Sie das Problem an den Microsoft-Support eskalieren:

1. Öffnen Sie das Postfach in Outlook im Internet, und klicken Sie auf **Einstellungen** \> **Optionen** \> **e-Mail-** \> **Posteingangsregeln**organisieren.

2. Klicken Sie unten auf der Seite auf **Wenn Ihre Regeln nicht funktionieren klicken Sie hier, um einen Diagnosebericht zu erstellen**.
