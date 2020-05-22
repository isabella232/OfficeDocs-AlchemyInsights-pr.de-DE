---
title: SharePoint-Benachrichtigungs Benachrichtigungen nicht zugestellt
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: 363f3c79a3b62f3017e6c873f1be3dd195cab883
ms.sourcegitcommit: 5296874062b16f945d9a7a7a9ab29ec53686310b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/21/2020
ms.locfileid: "44343095"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>SharePoint-Benachrichtigungs Benachrichtigungen nicht zugestellt

Überprüfen Sie den Ordner Junk in Ihrer e-Mail, da manchmal Warnungen möglicherweise dorthin gelangen.

Ermitteln Sie, ob **alle Warnungen nicht zugestellt werden** oder ob **eine einzelne Warnung** aus einer bestimmten Datei oder Bibliothek nicht zugestellt wird.

- **Einzelne Warnungen werden nicht zugestellt**: Wenn eine einzelne Warnung aus einer bestimmten Datei oder Bibliothek nicht zugestellt wird, können Sie versuchen, Sie zu löschen und neu zu erstellen. Informationen zum erneuten Erstellen der Benachrichtigung finden Sie unter [verwalten, anzeigen oder Löschen von SharePoint-Warnungen](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .
- **Alle Warnungen werden nicht zugestellt**: Wenn alle Warnungen aus mehreren Dateien oder Bibliotheken nicht zugestellt werden, besuchen Sie das [Service-Integritäts Dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , um nach eventuellen Ratschlägen/Vorfällen zu suchen, die mit SharePoint oder Exchange möglicherweise auftreten. Das Problem kann mit der SharePoint-Benachrichtigungsfunktion oder mit Verzögerungen in e-Mails durch Exchange auftreten. Es wird auch wichtig sein zu beachten, ob andere e-Mails zugestellt werden, und wenn nicht, ist das Problem wahrscheinlich bei Exchange-Verzögerungen.

FAQ für Benachrichtigungen:

- Es ist nicht möglich, Warnungen an die Verteilergruppe zu senden, sondern nur Sicherheits-und O365-Gruppen werden unterstützt.
- Sie können keine e-Mail-Benachrichtigungsvorlagen anpassen. Sie müssen Microsoft Flow oder SharePoint Designer Workflow verwenden, um diese zu erreichen.

## <a name="related-topics"></a>Verwandte Themen

Möchten Sie Microsoft Flow in SharePoint Online testen?

- [Fluss erstellen](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint und Flow](https://flow.microsoft.com//blog/sharepoint-and-flow/)
