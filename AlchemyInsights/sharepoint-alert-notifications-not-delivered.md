---
title: SharePoint-Benachrichtigungs Benachrichtigungen nicht zugestellt
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: d01d985f34d782fe14b3e2e6e6696c0101002db1
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36744640"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>SharePoint-Benachrichtigungs Benachrichtigungen nicht zugestellt

Überprüfen Sie den Ordner Junk in Ihrer e-Mail, da manchmal Warnungen möglicherweise dorthin gelangen.

Ermitteln Sie, ob **alle Warnungen nicht zugestellt werden** oder ob **eine einzelne Warnung** aus einer bestimmten Datei oder Bibliothek nicht zugestellt wird.

- **Einzelne Warnungen werden nicht zugestellt**: Wenn eine einzelne Warnung aus einer bestimmten Datei oder Bibliothek nicht zugestellt wird, können Sie versuchen, Sie zu löschen und neu zu erstellen. Informationen zum erneuten Erstellen der Benachrichtigung finden Sie unter [verwalten, anzeigen oder Löschen von SharePoint-Warnungen](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=&ad=US#ID0EAADAAA=Online) .
- **Alle Warnungen werden nicht zugestellt**: Wenn alle Warnungen aus mehreren Dateien oder Bibliotheken nicht zugestellt werden, besuchen Sie das [Service-Integritäts Dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , um nach eventuellen Ratschlägen/Vorfällen zu suchen, die mit SharePoint oder Exchange möglicherweise auftreten. Das Problem kann mit der SharePoint-Benachrichtigungsfunktion oder mit Verzögerungen in e-Mails durch Exchange auftreten. Es wird auch wichtig sein zu beachten, ob andere e-Mails zugestellt werden, und wenn nicht, ist das Problem wahrscheinlich bei Exchange-Verzögerungen.

FAQ für Benachrichtigungen:

- Es ist nicht möglich, Warnungen an die Verteilergruppe zu senden, sondern nur Sicherheits-und O365-Gruppen werden unterstützt.
- Sie können keine e-Mail-Benachrichtigungsvorlagen anpassen. Sie müssen Microsoft Flow oder SharePoint Designer Workflow verwenden, um diese zu erreichen.

Weitere Informationen:

- **Warnungs Setup**: Weitere Informationen zum Einrichten von Warnungen finden Sie unter [Erstellen einer Warnung, um benachrichtigt zu werden, wenn sich eine Datei oder ein Ordner in SharePoint ändert](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).
- **Problembehandlung bei Warnungen**: Weitere Informationen zur Problembehandlung bei Warnungen finden Sie unter [Benutzer erhalten keine SharePoint Online Benachrichtigungs Benachrichtigungen](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).
- **Richtlinien für erweiterte O365-Konformitäts**Warnungen: Weitere Informationen zum Einrichten dieser Warnungen finden Sie unter [Compliance Alert Policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies).
- **SharePoint-und OneDrive-Überwachungsprotokolle**: Weitere Informationen zum Abrufen dieser Ereignisse finden Sie unter [Durchsuchen des Überwachungsprotokolls](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
- **Von Advanced Threat Protection gesendete Warnungen**: siehe [ATP für SharePoint und OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).
- **Von Data Loss Prevention Policies gesendete Warnungen**: siehe [e-Mail-Benachrichtigungen für DLP-Richtlinien](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).

## <a name="related-topics"></a>Verwandte Themen

Möchten Sie Microsoft Flow in SharePoint Online testen?

- [Fluss erstellen](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint und Flow](https://flow.microsoft.com//blog/sharepoint-and-flow/)
