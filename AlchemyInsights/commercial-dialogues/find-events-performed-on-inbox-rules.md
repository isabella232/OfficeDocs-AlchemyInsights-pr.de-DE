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
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313498"
---
# <a name="find-events-performed-on-inbox-rules"></a>Suchen nach Ereignissen, die für Posteingangsregeln ausgeführt werden

Wenn Posteingangsregeln erstellt, geändert oder gelöscht werden, werden die Ereignisse im Überwachungsprotokoll aufgezeichnet. So überprüfen Sie sie:

1. Führen Sie eine der folgenden Aktionen aus:
   - Wechseln Sie im Microsoft 365 Compliance Center unter <https://compliance.microsoft.com> "Lösungsüberwachung" zu **"Lösungsüberwachung".** \>  Oder verwenden Sie , um direkt zur **Seite "Überwachung"** zu <https://compliance.microsoft.com/auditlogsearch> wechseln.
   - Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com> zu **"Überwachen".** Oder verwenden Sie , um direkt zur **Seite "Überwachung"** zu <https://security.microsoft.com/auditlogsearch> wechseln.

    **Hinweis:** Wenn Eine Benachrichtigung angezeigt wird, dass Sie die Überwachung aktivieren müssen, fahren Sie fort, und aktivieren Sie sie jetzt. Wenn dieses Feature nicht aktiviert ist, können Suchergebnisse keine Daten aus früheren Datumsangaben abrufen.
1. Wählen Sie das Feld "Aktivitäten" aus, suchen Sie Exchange Postfachaktivitäten, und wählen Sie dann New-InboxRule Posteingangsregel aus Outlook Web App erstellen aus. Wenn Sie fertig sind, klicken Sie außerhalb des Bereichs, um den Bereich "Aktivitäten" zu minimieren.
1. Geben Sie den Datumsbereich an, und wählen Sie dann im Feld "Benutzer" den Benutzernamen für den Benutzer aus, den Sie untersuchen möchten. Sie können mehrere Benutzer gleichzeitig auswählen.
1. Wählen Sie Suchen aus. Die Aktivitäten werden unter Ergebnisse angezeigt.
1. Um Details anzuzeigen, wählen Sie eine Aktivität und dann weitere Informationen aus. Im Abschnitt "Parameter" sehen Sie den Namen der Regel, die festgelegten Bedingungen und die Aktionen, die die Regel ausführt.

2. Konfigurieren Sie auf der Registerkarte **"Suchen"** der **Überwachungsseite** die folgenden Einstellungen:
   - **Datums- und Uhrzeitbereich:** Wählen Sie den Datums-/Uhrzeitbereich in den Feldern **Start** und Ende aus. 
   - **Aktivitäten:** Wählen Sie **"Neue Posteingangsregel erstellen" aus Outlook Web App**

3. Wenn Sie fertig sind, klicken Sie auf **Suchen.** Die Aktivitäten werden auf der neuen **Überwachungssuchseite** angezeigt.

4. Wählen Sie eine Aktivität in den Ergebnissen aus, um das Detail-Flyout zu öffnen. Im Abschnitt **"Parameter"** sehen Sie den Namen der Regel, die festgelegten Bedingungen und die Aktionen, die die Regel ausführt.

Weitere Informationen finden Sie unter [Durchsuchen des Überwachungsprotokolls, um allgemeine Supportprobleme zu untersuchen.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
