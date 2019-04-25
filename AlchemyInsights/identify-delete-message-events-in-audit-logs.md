---
title: Identifizieren von Ereignissen zum Löschen von Nachrichten in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32416709"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Überwachungsprotokolle für gelöschte e-Mail-Nachrichten

Ab Januar 2019 aktiviert Microsoft die postfachüberwachungsprotokollierung standardmäßig. Andernfalls müssen Sie die Löschaktionen für die Überwachung manuell aktivieren, um Lösch Nachrichten Ereignisse für einen bestimmten Benutzer zu überprüfen. Wenn die postfachüberwachungsprotokollierung für Ihre Organisation oder für den jeweiligen Benutzer bereits aktiviert ist, führen Sie die folgenden Schritte aus.

1. Melden Sie sich beim [Office 365 Security _AMP_ Compliance Center](https://protection.office.com/) an.

2. Klicken Sie auf **Suchen und Untersuchung** , und wählen Sie **Überwachungsprotokoll Suche**aus.

3. Wählen Sie den Datumsbereich in den Feldern **Start Datum** und Enddatum aus. **** Geben Sie username für den zu untersuchenden Benutzer an (der Benutzer, der die Elemente gelöscht hat). Wählen Sie im Feld **Aktivitäten** die Option **Gelöschte Nachrichten aus Ordner "Gelöschte Elemente" aus** , und **verschieben Sie Nachrichten in Ordner "Gelöschte Elemente"**.

4. Klicken Sie auf **Suchen**.

Wählen Sie in den Ergebnissen einen Überwachungsdatensatz aus. Klicken Sie im Detail Flyout auf **Weitere Informationen**. Zusätzliche Informationen zum gelöschten Element (beispielsweise die Betreffzeile und der Speicherort des Elements, wenn Sie gelöscht wurde) werden im Feld **AffectedItems** angezeigt. Die **ClientInfoString** -Eigenschaft zeigt an, ob der Löschvorgang in Outlook, Outlook im Web (früher als Outlook Web App bezeichnet) oder einem anderen Gerät stattgefunden hat.

Weitere Informationen finden Sie unter [bestimmen der Benutzer, die e-Mail-Weiterleitung für ein Postfach eingerichtet](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items)haben.

**Hinweis**: Gelöschte Elemente können nicht mithilfe des Überwachungsprotokoll Features abgerufen werden. Informationen zum Abrufen von gelöschten Nachrichten in Outlook im Web finden Sie unter [Recover Deleted Items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
