---
title: Dynamics 365-falsche Dashboard-Shows in Dynamics 365 Unified Interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/25/2019
ms.locfileid: "36528550"
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
