---
title: Workflow wird nicht gestartet
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 77a3c022a9a3a82041b4a4a70c72c2e0940c0fba27f296f07881e3abebf1e464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53907737"
---
# <a name="workflow-is-not-starting"></a>Workflow wird nicht gestartet

- SharePoint 2010- und SharePoint 2013-Workflows werden nicht gestartet.

    - Wenn Ihr Workflow nicht gestartet wird, kann es zu einem temporären Dienstproblem kommen, bei dem Es bei Benutzern zu zeitweiligen Verzögerungen beim Workflowfortschritt kommen kann. Überprüfen Sie das [Dienststatus-Dashboard,](https://admin.microsoft.com/AdminPortal/Home/servicehealth) um festzustellen, ob Ihre Organisation betroffen ist.

    - Wenn seit dem ersten Auftreten dieses Problems mehr als 24 Stunden vergangen sind, melden Sie sich bitte ein Supportticket an. In vielen Fällen arbeiten wir bereits an einer Lösung. Bitte geben Sie uns mindestens 24 Stunden Zeit, um eine Lösung abzuschließen.

- SharePoint 2010-Workflows wurden beim Start verzögert.

    - Dies tritt auf, wenn der Workflow in großen Batches ausgelöst wird. (z. B. wenn mehrere Elemente gleichzeitig hinzugefügt werden).

    - Workflows sind nicht für die Ausführung in Echtzeit ausgelegt, daher ist eine Verzögerung das Entwurfsverhalten.

   -  Wenn der Workflow eine komplexe Extensible Object Markup Language (XSTYLE) ist, kann die Kompilierung langsam sein. Lesen Sie [diesen](https://support.microsoft.com//kb/3043697) Artikel.

    - Sie sollten den Workflow vereinfachen oder mithilfe des Microsoft SharePoint 2013-Workflowplattformtyps neu entwerfen.

    - Wenn ihr Workflowverlauf sehr umfangreich ist, können Sie die Elemente löschen oder eine neue Verlaufsliste erstellen.

        Weitere Informationen: [Löschen des Workflowverlaufs](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Verwandte Themen
Möchten Sie Microsoft Flow in SharePoint Online testen?
- [Erstellen Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint und Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
