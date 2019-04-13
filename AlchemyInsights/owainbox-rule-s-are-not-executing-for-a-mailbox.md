---
title: 1332 OWA-postEingangsregel (n) werden nicht für ein Postfach ausgeführt
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: c0b221b5335254bd0f1eb4b258efa6946376ca12
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858743"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Eine postEingangsregel funktioniert nicht wie erwartet

Überprüfen Sie die folgenden Einstellungen:

- Eine Nachricht kann nur einmal auf Basis von postEingangsregeln umgeleitet, weitergeleitet oder beantwortet werden. Eine Umleitungsregel (eine postEingangsregel oder eine Nachrichtenfluss Regel, auch als Transportregel bezeichnet) kann maximal zehn Weiterleitungs Empfänger zu einer Nachricht hinzufügen. Weitere Informationen finden Sie unter [Journal-, Transport-und Posteingangsregel Limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- PostEingangsregeln funktionieren nicht für das alternative Journalpostfach. Weitere Informationen zum alternativen Journalpostfach finden Sie unter alternatives [Journalpostfach](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Um diese Probleme zu beheben, lesen Sie [KB 2829319](https://support.microsoft.com/kb/2829319).

Wenn die vorherigen Probleme nicht zutreffen, führen Sie den Diagnosebericht "postEingangsregel" aus, bevor Sie das Problem an den Microsoft-Support eskalieren:

1. Öffnen Sie das Postfach in Outlook im Web, und klicken Sie auf **Einstellungen** \> **Optionen** \> **Organisieren von e-Mail-** \> **Posteingangsregeln**.

2. Klicken Sie unten auf der Seite auf, **Wenn Ihre Regeln nicht funktionieren klicken Sie hier, um einen Diagnosebericht zu generieren**.
