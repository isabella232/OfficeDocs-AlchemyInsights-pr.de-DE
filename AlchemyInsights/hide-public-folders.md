---
title: Öffentliche Ordner ausblenden
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/18/2021
ms.locfileid: "50294642"
---
# <a name="hide-public-folders"></a>Öffentliche Ordner ausblenden

**So blenden Sie die gesamte öffentliche Ordnerstruktur aus**:

Verwenden Sie die Schritte in [diesem](https://aka.ms/ControlPF) Artikel, um die gesamte öffentliche Ordnerstruktur vor ausgewählten oder allen Benutzern zu verbergen.

**So blenden Sie einen bestimmten öffentlichen Ordner aus**:

1. Hinzufügen von Berechtigungen für Benutzer, die auf den öffentlichen Ordner zugreifen müssen

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Entfernen Sie den Benutzer **Standard** aus der **Berechtigungsliste**:

    `Remove-PublicFolderClientPermission \test1 -User Default`
