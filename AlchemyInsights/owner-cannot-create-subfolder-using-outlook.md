---
title: Besitzer kann keinen Unterordner mit Outlook erstellen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/12/2020
ms.locfileid: "44716598"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Besitzer kann keinen Unterordner mit Outlook erstellen

**Es gibt ein anhaltendes Problem mit Besitzern öffentlicher Ordner, die Unterordner mit Outlook erstellen. Das Problem wird in Kürze behoben.**

In der Zwischenzeit können Sie eine der folgenden Problemumgehungen verwenden:

1. Verwenden Sie Outlook für MAC, um den Unterordner zu erstellen, da das Problem nur Outlook für Desktop-Fenster betrifft (alle Versionen)
2. Lassen Sie den Administrator den Unterordner mit EXO Shell oder EAC erstellen
3. Ändern von DefaultPublicFolderMailbox/EffectivePublicFolderMailbox des Benutzers in ein anderes Postfach als das Inhaltspostfach für den Ordner, der das Problem verursacht  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Warten Sie eine Stunde, und starten Sie den Outlook-Client erneut