---
title: 1332 OWA - Posteingang Regeln nicht für ein Postfach ausgeführt werden
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f090d0a9d84bc6a4d1a1f4c0af55102d4b0ddfbe
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28289958"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Eine Posteingangsregel funktioniert nicht wie erwartet

Überprüfen Sie die folgenden Einstellungen:
  
- Eine Nachricht kann weitergeleitete oder beantwortete automatisch basierend auf Posteingangsregeln nur einmal umgeleitet werden. Eine umleiten Regel (Posteingangsregel oder e-Mail-Flussregel, auch bekannt als eine Transportregel) kann maximal 10 Weiterleitung der Empfänger einer Nachricht hinzufügen. Weitere Informationen finden Sie unter [Journal, Transport, und Posteingang Regel Grenzwerte](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).
    
- Posteingangsregeln funktionieren nicht auf die alternatives Journalpostfach. Weitere Informationen zu den alternatives Journalpostfach finden Sie unter [alternatives Journalpostfach](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).
    
Zum Beheben dieser Probleme finden Sie unter [KB 2829319](https://support.microsoft.com/kb/2829319).
  
Wenn die vorherigen Problemen nicht angewendet werden, führen Sie den Posteingang Regel Diagnosebericht, bevor Sie das Problem an Microsoft Support ausweiten:
  
1. Öffnen Sie das Postfach in Outlook im Web, und klicken Sie auf **Einstellungen** \> **Optionen** \> **Organisieren e-Mail** \> **Posteingangsregeln**.
    
2. Klicken Sie am unteren Rand der Seite **Wenn Ihre Regeln klicken Sie hier, um einen Diagnosebericht generieren nicht funktionieren**.
    

