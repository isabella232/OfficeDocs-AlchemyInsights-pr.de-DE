---
title: Suchen nach Ereignissen, die für Posteingangsregeln ausgeführt werden
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 14a5a18bc1422572db567c9533fefe5a7e0120afd64df4a64623038cc063ce93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058649"
---
# <a name="find-events-performed-on-inbox-rules"></a>Suchen nach Ereignissen, die für Posteingangsregeln ausgeführt werden

Wenn Posteingangsregeln erstellt, geändert oder gelöscht werden, werden die Ereignisse im Überwachungsprotokoll aufgezeichnet. Hier erfahren Sie, wie Sie diese überprüfen:

1. Wechseln Sie zum [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Wählen Sie "Suchen > Überwachungsprotokollsuche" aus.

    > [!NOTE]
    > Wenn Sie einen Hinweis sehen, dass Sie die Überwachung aktivieren müssen, fahren Sie fort, und aktivieren Sie sie jetzt. Wenn dieses Feature nicht aktiviert ist, können Suchergebnisse keine Daten aus früheren Datumsangaben abrufen.
1. Wählen Sie das Feld "Aktivitäten" aus, suchen Sie Exchange Postfachaktivitäten, und wählen Sie dann New-InboxRule Posteingangsregel aus Outlook Web App. Wenn Sie fertig sind, klicken Sie außerhalb des Bereichs, um den Bereich "Aktivitäten" zu minimieren.
1. Geben Sie den Datumsbereich an, und wählen Sie dann im Feld "Benutzer" den Benutzernamen für den Benutzer aus, den Sie untersuchen möchten. Sie können mehrere Benutzer gleichzeitig auswählen.
1. Wählen Sie Suchen aus. Die Aktivitäten werden unter Ergebnisse angezeigt.
1. Um Details anzuzeigen, wählen Sie eine Aktivität und dann weitere Informationen aus. Im Abschnitt "Parameter" sehen Sie den Namen der Regel, die festgelegten Bedingungen und die Aktionen, die die Regel ausführt.

Weitere Informationen finden Sie unter Durchsuchen des Office 365 Überwachungsprotokolls, um häufige Szenarien zu beheben.