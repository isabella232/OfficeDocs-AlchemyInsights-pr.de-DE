---
title: Wiederherstellen eines gelöschten öffentlichen Ordners
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774530"
---
# <a name="restore-a-deleted-public-folder"></a>Wiederherstellen eines gelöschten öffentlichen Ordners

**So stellen Sie gelöschte Elemente in einem öffentlichen Ordner wieder her**:

- Weitere Informationen finden [Sie unter Sie können gelöschte Elemente nicht aus einem öffentlichen Ordner außerhalb von e-Mail in Outlook 2016 wiederherstellen](https://aka.ms/pfrec).
 
**So stellen Sie einen gelöschten öffentlichen Ordner (eines beliebigen Typs) wieder her**: 

- Verwenden Sie den folgenden Exo PowerShell-Befehl:

    Syntax:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Beispiel: mit dem folgenden Befehl wird Unterordner1 wiederhergestellt und unter \Parent1 platziert:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Weitere Informationen finden Sie unter [Wiederherstellen eines gelöschten öffentlichen Ordners](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
