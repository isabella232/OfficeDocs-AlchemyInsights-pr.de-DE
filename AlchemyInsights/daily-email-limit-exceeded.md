---
title: Grenzwert für tägliche e-Mail überschritten. Workflow ist angehalten.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053116"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Grenzwert für tägliche e-Mail überschritten. Workflow ist angehalten.

Dieser Fehler kann in den folgenden Szenarien eingegangen sein:

- Sie verfügen über einen Workflow in SharePoint Online, der den SharePoint 2010 oder SharePoint 2013 Workflow-Plattformtyp verwendet.
- Der Workflow ist so konfiguriert, dass eine benutzerdefinierte e-Mail-Nachricht an mehr als 200 Benutzer gleichzeitig gesendet wird, mehr als 10.000 Empfänger pro Tag oder mehr als 30 Nachrichten pro Minute.
- Wenn Sie den Workflow ausführen, wird die e-Mail-Nachricht nicht gesendet, und Sie sehen das folgende Verhalten:
    - Für einen Workflow mithilfe des SharePoint 2013 Plattformtyps navigieren Sie zur Seite **Workflow Status** . Auf der Seite Workflow Status ist der **interne Status** auf **gestartet**festgelegt, und die Informations Sprechblase zeigt an, dass **keine Empfänger gesendet**werden können.

Um dieses Problem zu umgehen, konfigurieren Sie Ihren Workflow zum Senden von e-Mail-Nachrichten, ohne die [Exchange Online Absender Grenzwerte](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)zu überschreiten. Verwenden Sie beispielsweise eine Pause im Workflow, senden Sie die e-Mail an eine Office 365 Gruppe, eine Verteilergruppe oder eine e-Mail-aktivierte Sicherheitsgruppe, oder senden Sie die Nachricht an weniger als 200 Empfänger gleichzeitig.


Weitere Informationen finden Sie im folgenden [Artikel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Verwandte Themen
- [Fluss erstellen](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint und Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 