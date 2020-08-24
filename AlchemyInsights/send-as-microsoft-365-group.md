---
title: Senden als Microsoft 365-Gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2020
ms.locfileid: "46853001"
---
# <a name="send-as-microsoft-365-group"></a>Senden als Microsoft 365-Gruppe

Sie können "Senden als"-Berechtigungen zuweisen, um bestimmten Benutzern das Senden von Nachrichten als Microsoft 365-Gruppe zu erlauben:  

1. Stellen Sie eine Verbindung mit Exchange Online PowerShell her.  

2. Führen Sie den folgenden Befehl aus:  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs

Weitere Informationen finden Sie unter [Zulassen, dass Mitglieder mit "Senden als" oder "Senden im Auftrag von" E-Mails für eine Gruppe senden](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).