---
title: Senden als Microsoft 365-Gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 51bd8a10c3da23941cc16d7ba860406f8477044a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740150"
---
# <a name="send-as-microsoft-365-group"></a>Senden als Microsoft 365-Gruppe

Sie können "Senden als"-Berechtigungen zuweisen, um bestimmten Benutzern das Senden von Nachrichten als Microsoft 365-Gruppe zu erlauben:  

1. Stellen Sie eine Verbindung mit Exchange Online PowerShell her.  

2. Führen Sie den folgenden Befehl aus:  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs

Weitere Informationen finden Sie unter [Zulassen, dass Mitglieder mit "Senden als" oder "Senden im Auftrag von" E-Mails für eine Gruppe senden](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).