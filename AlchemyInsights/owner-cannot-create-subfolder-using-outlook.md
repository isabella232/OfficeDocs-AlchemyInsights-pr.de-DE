---
title: Besitzer kann keinen Unterordner mit Outlook erstellen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836134"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Besitzer kann keinen Unterordner mit Outlook erstellen

**Es gibt ein anhaltendes Problem mit Besitzern öffentlicher Ordner, die Unterordner mit Outlook erstellen. Das Problem wird in Kürze behoben.**

In der Zwischenzeit können Sie eine der folgenden Problemumgehungen verwenden:

1. Verwenden Sie Outlook für MAC, um den Unterordner zu erstellen, da das Problem nur Outlook für Desktop-Fenster betrifft (alle Versionen)
2. Lassen Sie den Administrator den Unterordner mit EXO Shell oder EAC erstellen
3. Ändern von DefaultPublicFolderMailbox/EffectivePublicFolderMailbox des Benutzers in ein anderes Postfach als das Inhaltspostfach für den Ordner, der das Problem verursacht  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Warten Sie eine Stunde, und starten Sie den Outlook-Client erneut