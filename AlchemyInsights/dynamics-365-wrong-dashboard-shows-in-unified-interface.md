---
title: Dynamics 365-falsche Dashboard-Shows in Dynamics 365 Unified Interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711274"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Falsche Dashboard-Anzeige in Dynamics 365 Unified Interface

Es gibt mehrere Gründe, aus denen Sie ein anderes Dashboard als das erwartete anzeigen können:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Der Benutzer hat ein Standarddashboard für Benutzer festgelegt. 

Normalerweise können Sie angeben, dass ein Benutzer Standarddashboard festgelegt wird, wenn die Schaltfläche **als Standard festlegen** in der Befehlsleiste des Dashboards nicht angezeigt wird. Das Standarddashboard des Benutzers setzt alle anderen Standard Dashboards außer Kraft, auch wenn sich das Standarddashboard des Benutzers nicht in der aktuellen App befindet.

Verwenden Sie die folgende Problemumgehung, um Ihr Standarddashboard zu löschen.

1. Erstellen Sie ein neues persönliches Dashboard.

2. Legen Sie das neue Dashboard als Benutzer Standard fest.

3. Löschen Sie das Dashboard.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Das Dashboard wird in der Sitemap festgelegt.

Sie haben möglicherweise ein Standarddashboard für die Organisation festgelegt, indem Sie ein Dashboard auswählen und "als Standard festlegen" unter "System anpassen" auswählen. Das im Sitemap-Designer definierte Dashboard hat jedoch Vorrang vor diesem Dashboard, wenn der Benutzer darauf zugreifen kann.

Um Benutzern das als Organisationsstandard festgelegte Dashboard anzuzeigen, können Sie entweder:

* Festlegen des Dashboards in der Sitemap

* Entfernen des Zugriffs auf das definierte Sitemap-Dashboard für diese Benutzer
