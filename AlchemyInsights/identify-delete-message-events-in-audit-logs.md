---
title: Identifizieren von Ereignissen zum Löschen von Nachrichten in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: b358b7944b82182a8551d64701e6879a01816524
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539208"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Überwachungsprotokolle für gelöschte e-Mail-Nachrichten

Ab Januar 2019 wendet Microsoft die postfachüberwachungsprotokollierung standardmäßig an. Andernfalls müssen Sie die Löschaktionen für die Überwachung manuell aktivieren, um Lösch Nachrichten Ereignisse für einen bestimmten Benutzer zu überprüfen. Wenn die postfachüberwachungsprotokollierung bereits für Ihre Organisation oder für den jeweiligen Benutzer aktiviert ist, führen Sie die folgenden Schritte aus.

1. Melden Sie sich beim [Office 365 Security #a0 Compliance Center](https://protection.office.com/) an.

2. Klicken Sie auf **Suche und Untersuchung** , und wählen Sie **Überwachungsprotokoll Suche**aus.

3. Wählen Sie den Datumsbereich in den Feldern **Start Datum** und Enddatum aus. **** Geben Sie den Benutzernamen für den Benutzer an, der untersucht werden soll (der Benutzer, der die Elemente gelöscht hat). Wählen Sie im Feld **Aktivitäten** die Option **Gelöschte Nachrichten aus dem Ordner "Gelöschte Elemente" aus** , und **Verschieben von Nachrichten in den Ordner "Gelöschte Elemente"**.

4. Klicken Sie auf **Suchen**.

Wählen Sie in den Ergebnissen einen Überwachungseintrag aus. Klicken Sie im Detail Flyout auf **Weitere Informationen**. Weitere Informationen zum gelöschten Element (beispielsweise die Betreffzeile und der Speicherort des Elements, wenn es gelöscht wurde) werden im Feld **AffectedItems** angezeigt. Die **ClientInfoString** -Eigenschaft zeigt an, ob der Löschvorgang in Outlook, Outlook im Internet (früher bekannt als Outlook Web App) oder auf einem anderen Gerät aufgetreten ist.

Weitere Informationen finden Sie unter [bestimmen der Personen, die die e-Mail-Weiterleitung für ein Postfach eingerichtet](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items)haben.

**Hinweis**: Gelöschte Elemente können nicht mithilfe der Überwachungsprotokoll Funktion abgerufen werden. Informationen zum Abrufen von gelöschten Nachrichten in Outlook im Internet finden Sie unter [Wiederherstellen gelöschter Elemente in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
