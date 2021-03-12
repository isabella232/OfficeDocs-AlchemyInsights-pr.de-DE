---
title: Fix user policy/mailbox settings
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737130"
---
# <a name="fix-user-policymailbox-settings"></a>Fix user policy/mailbox settings

Die Junk-E-Mail-Einstellungen für das Postfach haben diese Nachricht beeinflusst. Gehen Sie wie folgt vor, um die Einstellungen zu überprüfen:

1. Starten Sie die Exchange-Verwaltungsshell. Weitere Informationen finden Sie unter [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Führen Sie diesen Befehl aus (unter Verwendung der  **E-Mail-Adresse des Benutzers): get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Überprüfen Sie, ob die E-Mail-Adresse des Absenders Teil von **TrustedSendersAndDomains** oder **BlockedSendersAndDomains ist.** Wenn sich die E-Mail-Adresse in einer der Listen befindet, müssen Sie sie möglicherweise entfernen. Weitere Informationen finden Sie unter [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
