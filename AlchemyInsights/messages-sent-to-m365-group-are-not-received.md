---
title: An eine Microsoft 365-Gruppe gesendete Nachrichten werden nicht von allen Mitgliedern empfangen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: d2f0674f6be135927dc5995575c14f3c2708df49
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806146"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="c70d3-102">An eine Microsoft 365-Gruppe gesendete Nachrichten werden nicht von allen Mitgliedern empfangen</span><span class="sxs-lookup"><span data-stu-id="c70d3-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="c70d3-103">Stellen Sie sicher, dass alle Gruppenmitglieder den Empfang der E-Mails abonniert haben.</span><span class="sxs-lookup"><span data-stu-id="c70d3-103">Make sure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="c70d3-104">Siehe [Folgen einer Gruppe in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span><span class="sxs-lookup"><span data-stu-id="c70d3-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="c70d3-105">Um den Nachrichtenstatus von Mitgliedern zu überprüfen, die Gruppen-E-Mails abonniert haben, führen Sie den folgenden Befehl in [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps) aus:</span><span class="sxs-lookup"><span data-stu-id="c70d3-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`