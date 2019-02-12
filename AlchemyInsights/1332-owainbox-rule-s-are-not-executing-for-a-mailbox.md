---
title: 1332 OWA - Posteingang Regeln nicht für ein Postfach ausgeführt werden
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 0d3b7ce3d6b32d94a012eb3767c0747eed80f6e5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29915803"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Eine Posteingangsregel funktioniert nicht wie erwartet

Überprüfen Sie die folgenden Einstellungen:
  
- Eine Nachricht kann weitergeleitete oder beantwortete automatisch basierend auf Posteingangsregeln nur einmal umgeleitet werden. Eine umleiten Regel (Posteingangsregel oder e-Mail-Flussregel, auch bekannt als eine Transportregel) kann maximal 10 Weiterleitung der Empfänger einer Nachricht hinzufügen. Weitere Informationen finden Sie unter [Journal, Transport, und Posteingang Regel Grenzwerte](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).
    
- Posteingangsregeln funktionieren nicht auf die alternatives Journalpostfach. Weitere Informationen zu den alternatives Journalpostfach finden Sie unter [alternatives Journalpostfach](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).
    
Zum Beheben dieser Probleme finden Sie unter [KB 2829319](https://support.microsoft.com/kb/2829319).
  
Wenn die vorherigen Problemen nicht angewendet werden, führen Sie den Posteingang Regel Diagnosebericht, bevor Sie das Problem an Microsoft Support ausweiten:
  
1. Öffnen Sie das Postfach in Outlook im Web, und klicken Sie auf **Einstellungen** \> **Optionen** \> **Organisieren e-Mail** \> **Posteingangsregeln**.
    
2. Klicken Sie am unteren Rand der Seite **Wenn Ihre Regeln klicken Sie hier, um einen Diagnosebericht generieren nicht funktionieren**.
    

