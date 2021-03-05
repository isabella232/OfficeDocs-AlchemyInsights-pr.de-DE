---
title: Suchen von Ereignissen, die für Posteingangsregeln ausgeführt werden
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464703"
---
# <a name="find-events-performed-on-inbox-rules"></a>Suchen von Ereignissen, die für Posteingangsregeln ausgeführt werden

Wenn Posteingangsregeln erstellt, geändert oder gelöscht werden, werden die Ereignisse im Überwachungsprotokoll aufgezeichnet. Hier erfahren Sie, wie Sie sie überprüfen:

1. Wechseln Sie zum [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Wählen Sie Suchen > Überwachungsprotokollsuche aus.

    > [!NOTE]
    > Wenn Sie eine Benachrichtigung sehen, dass Sie die Überwachung aktivieren müssen, fahren Sie mit der Überwachung voran, und aktivieren Sie sie jetzt. Wenn dieses Feature nicht aktiviert ist, können Suchergebnisse keine Daten aus früheren Datumsangaben ziehen.
1. Wählen Sie das Feld Aktivitäten aus, und suchen Sie nach Exchange-Postfachaktivitäten, und wählen Sie dann New-InboxRule Posteingangsregel in Outlook Web App erstellen aus. Wenn Sie fertig sind, klicken Sie außerhalb des Bereichs, um den Bereich Aktivitäten zu minimieren.
1. Geben Sie den Datumsbereich an, und wählen Sie dann im Feld Benutzer den Benutzernamen für den Benutzer aus, den Sie untersuchen möchten. Sie können mehrere Benutzer gleichzeitig auswählen.
1. Wählen Sie Suchen aus. Die Aktivitäten werden unter Ergebnisse angezeigt.
1. Um Details anzuzeigen, wählen Sie eine Aktivität aus, und wählen Sie dann Weitere Informationen aus. Im Abschnitt Parameter sehen Sie den Namen der Regel, die festgelegten Bedingungen und die Aktionen, die die Regel ausführen wird.

Weitere Informationen finden Sie unter Durchsuchen des Office 365-Überwachungsprotokolls zur Problembehandlung gängiger Szenarien.