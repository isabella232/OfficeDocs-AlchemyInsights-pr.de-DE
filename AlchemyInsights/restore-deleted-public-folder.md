---
title: Wiederherstellen eines gelöschten öffentlichen Ordners
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809438"
---
# <a name="restore-a-deleted-public-folder"></a>Wiederherstellen eines gelöschten öffentlichen Ordners

**So stellen Sie gelöschte Elemente aus einem öffentlichen Ordner wieder auf:**

- Weitere Informationen finden Sie unter Sie können gelöschte Elemente aus einem öffentlichen Ordner ohne [E-Mail in Outlook 2016 nicht wiederherstellen.](https://aka.ms/pfrec)
 
**So stellen Sie einen gelöschten öffentlichen Ordner (beliebigen Typs) wieder auf:** 

- Verwenden Sie den folgenden EXO PowerShell-Befehl:

    Syntax:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Beispiel: Mit dem folgenden Befehl wird Subfolder1 wiederhergestellt und unter \Parent1 gespeichert:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Weitere [Informationen finden Sie unter Wiederherstellen eines gelöschten öffentlichen](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) Ordners.
