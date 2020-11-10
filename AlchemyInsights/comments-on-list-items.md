---
title: Kommentare zu Listenelementen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947508"
---
# <a name="comments-on-list-items"></a>Kommentare zu Listenelementen

Benutzer werden in Kürze Kommentare zu Listenelementen hinzufügen und löschen können. Benutzer können alle Kommentare zu einem Listenelement anzeigen und zwischen Ansichten filtern, die Kommentare oder Aktivitäten im Zusammenhang mit einem Element anzeigen.

**Timing** :

**Targeted Release** : schrittweiser Rollout Mitte Oktober und voraussichtlich bis Mitte November abgeschlossen

**Standard Version** : schrittweiser Rollout Mitte November und voraussichtlich bis Anfang Dezember abgeschlossen

**Rollout** : gezielte Freigabe für die gesamte Organisation

Benutzer müssen Folgendes beachten, bevor Sie Kommentare hinzufügen und löschen können:

- Kommentare entsprechen den Berechtigungseinstellungen von SharePoint.
- Klassische Listen, die noch nicht für die Darstellung in modernen Benutzeroberflächen wie Aufgabenlisten erstellt wurden, verfügen nicht über diese Kommentarfunktion.
- Das Kommentieren von Listen in Microsoft Teams steht in dieser Version nicht zur Verfügung.
- Kommentare werden nicht durch die Suche indiziert.

Administratoren können dieses Feature auf Organisationsebene deaktivieren, indem Sie den Parameter **CommentsOnListItemsDisabled** im PowerShell-Cmdlet " **Sets-SPOTenant** " ändern.

Es ist derzeit nicht möglich, das kommentieren auf Website-oder Listenebene zu deaktivieren. Wir hoffen, diese Steuerelemente in einem späteren Update zu haben, wahrscheinlich im ersten Quartal 2021.
