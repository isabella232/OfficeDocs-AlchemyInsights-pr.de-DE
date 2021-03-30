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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403742"
---
# <a name="workflow-is-not-starting"></a>Workflow wird nicht gestartet

- SharePoint 2010- und SharePoint 2013-Workflows werden nicht gestartet.

    - Wenn Der Workflow nicht gestartet wird, kann es zu einem temporären Dienstproblem kommen, bei dem Benutzer zeitweise Verzögerungen mit dem Workflowfortschritt erleben können. Überprüfen Sie [das Dienstintehashboard,](https://admin.microsoft.com/AdminPortal/Home/servicehealth) um zu sehen, ob Ihre Organisation betroffen ist.

    - Wenn seit dem ersten Problem mehr als 24 Stunden vergangen sind, protokollieren Sie bitte ein Supportticket. In vielen Fällen arbeiten wir bereits an einer Lösung. Bitte geben Sie uns mindestens 24 Stunden Zeit, um eine Lösung zu vervollständigen.

- SharePoint 2010-Workflows verzögerten sich beim Start.

    - Dies tritt auf, wenn der Workflow in großen Batches ausgelöst wird. (z. B. wenn mehrere Elemente gleichzeitig hinzugefügt werden).

    - Workflows sind nicht so konzipiert, dass sie in Echtzeit ausgeführt werden, daher ist eine Verzögerung ein by-design-Verhalten.

   -  Wenn der Workflow eine komplexe Extensible Object Markup Language (XMOL) ist, kann die Kompilierung langsam sein. Lesen [Sie diesen](https://support.microsoft.com//kb/3043697) Artikel.

    - Sie sollten den Workflow vereinfachen oder mithilfe des Microsoft SharePoint 2013-Workflowplattformtyps neu gestalten.

    - Wenn Ihr Workflowverlauf größer geworden ist, können Sie die Elemente löschen oder eine neue Verlaufsliste erstellen.

        Weitere Informationen : [Löschen des Workflowverlaufs](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Verwandte Themen
Möchten Sie Microsoft Flow in SharePoint Online testen?
- [Erstellen von Fluss](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint und Fluss](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
