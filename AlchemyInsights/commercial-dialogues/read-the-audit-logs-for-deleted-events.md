---
title: Lesen der Überwachungsprotokolle für gelöschte Ereignisse
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
ms.openlocfilehash: 8d656d5660b7c6e6d32d32a06c3dbf49c45e4ca04c4422128f1c4ea62413afa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53967332"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Lesen der Überwachungsprotokolle für gelöschte Ereignisse

So gehen Sie wie folgt vor:

1. Wechseln Sie zum [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Wählen Sie   >  [**"Überwachungsprotokollsuche durchsuchen" aus.**](https://go.microsoft.com/fwlink/?linkid=2103759)
    > [!NOTE]
    > Wenn Sie einen Hinweis sehen, dass Sie das Feature aktivieren müssen, fahren Sie fort, und aktivieren Sie es jetzt. Wenn das Feature nicht aktiviert ist, können Suchergebnisse keine Daten aus früheren Datumsangaben abrufen.
1. Wählen Sie **"Aktivitäten"** aus, und suchen Sie dann **nach Exchange Postfachaktivitäten.** Wählen Sie die Optionen **"Gelöschte Nachrichten" aus dem Ordner "Gelöschte Elemente"** und "Nachrichten in Ordner **"Gelöschte Elemente" verschieben** aus. Wenn Sie fertig sind, klicken Sie außerhalb des Bereichs, um den **Bereich "Aktivitäten"** zu minimieren.
1. Geben Sie den Datumsbereich an, und wählen Sie dann im Feld **"Benutzer"** den Benutzernamen für den Benutzer aus, den Sie untersuchen möchten. Sie können mehrere Benutzer gleichzeitig auswählen.
1. Wählen Sie **Suchen** aus. Die Aktivitäten werden unter **Ergebnisse** angezeigt.
1. Um die Details anzuzeigen, wählen Sie eine Aktivität aus, und wählen Sie dann **weitere Informationen** aus. Zusätzliche Informationen zum gelöschten Element, z. B. die Betreffzeile und den Speicherort des Elements, als es gelöscht wurde, werden im **Feld "AffectedItems"** angezeigt.
    > [!NOTE]
    > Gelöschte Elemente können nicht mithilfe der Überwachungsprotokollfunktion wiederhergestellt werden. Informationen zum Wiederherstellen gelöschter Elemente finden Sie unter [Wiederherstellen gelöschter Elemente oder E-Mails in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).

Weitere Informationen finden Sie unter [Durchsuchen des Office 365 Überwachungsprotokolls, um häufige Szenarien zu behandeln.](https://go.microsoft.com/fwlink/?linkid=2103944)
