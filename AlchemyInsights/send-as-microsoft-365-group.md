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
# <a name="send-as-microsoft-365-group"></a><span data-ttu-id="f096c-102">Senden als Microsoft 365-Gruppe</span><span class="sxs-lookup"><span data-stu-id="f096c-102">Send As Microsoft 365 group</span></span>

<span data-ttu-id="f096c-103">Sie können "Senden als"-Berechtigungen zuweisen, um bestimmten Benutzern das Senden von Nachrichten als Microsoft 365-Gruppe zu erlauben:</span><span class="sxs-lookup"><span data-stu-id="f096c-103">You can assign Send As permissions to allow specific users to send messages as a Microsoft 365 group:</span></span>  

1. <span data-ttu-id="f096c-104">Stellen Sie eine Verbindung mit Exchange Online PowerShell her.</span><span class="sxs-lookup"><span data-stu-id="f096c-104">Connect to Exchange Online PowerShell.</span></span>  

2. <span data-ttu-id="f096c-105">Führen Sie den folgenden Befehl aus:</span><span class="sxs-lookup"><span data-stu-id="f096c-105">Run the following command:</span></span>  

    <span data-ttu-id="f096c-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span><span class="sxs-lookup"><span data-stu-id="f096c-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span></span>

<span data-ttu-id="f096c-107">Weitere Informationen finden Sie unter [Zulassen, dass Mitglieder mit "Senden als" oder "Senden im Auftrag von" E-Mails für eine Gruppe senden](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="f096c-107">For more information, see [Allow members to send as or send on behalf of a group](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span></span>