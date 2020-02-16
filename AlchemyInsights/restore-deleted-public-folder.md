---
title: Wiederherstellen eines gelöschten öffentlichen Ordners
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063652"
---
# <a name="restore-a-deleted-public-folder"></a>Wiederherstellen eines gelöschten öffentlichen Ordners

**So stellen Sie gelöschte Elemente in einem öffentlichen Ordner wieder her**:

- Weitere Informationen finden [Sie unter Sie können gelöschte Elemente nicht aus einem öffentlichen Ordner außerhalb von e-Mail in Outlook 2016 wiederherstellen](https://aka.ms/pfrec).
 
**So stellen Sie einen gelöschten öffentlichen Ordner (eines beliebigen Typs) wieder her**: 

- Verwenden Sie den folgenden Exo PowerShell-Befehl:

    Syntax:

    >$PF = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-Rekursion |? {$_. Name-EQ "\<name_of_deleted_public_Folder"}; Festlegen-PublicFolder $PF. Identity-Path \<-Pfad, in dem der Ordner wiederhergestellt wird>

    Beispiel: mit dem folgenden Befehl wird Unterordner1 wiederhergestellt und unter \Parent1 platziert:

    >$PF = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-Rekursion |? {$_. Name-EQ "Unterordner1"}; Gruppe-PublicFolder $PF. Identity-Path \Parent1

Weitere Informationen finden Sie unter [Wiederherstellen eines gelöschten öffentlichen Ordners](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
