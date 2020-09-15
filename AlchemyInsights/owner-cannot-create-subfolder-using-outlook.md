---
title: Besitzer kann keinen Unterordner mit Outlook erstellen
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665717"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="1a697-102">Besitzer kann keinen Unterordner mit Outlook erstellen</span><span class="sxs-lookup"><span data-stu-id="1a697-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="1a697-103">**Es gibt ein anhaltendes Problem mit Besitzern öffentlicher Ordner, die Unterordner mit Outlook erstellen. Das Problem wird in Kürze behoben.**</span><span class="sxs-lookup"><span data-stu-id="1a697-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="1a697-104">In der Zwischenzeit können Sie eine der folgenden Problemumgehungen verwenden:</span><span class="sxs-lookup"><span data-stu-id="1a697-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="1a697-105">Verwenden Sie Outlook für MAC, um den Unterordner zu erstellen, da das Problem nur Outlook für Desktop-Fenster betrifft (alle Versionen)</span><span class="sxs-lookup"><span data-stu-id="1a697-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="1a697-106">Lassen Sie den Administrator den Unterordner mit EXO Shell oder EAC erstellen</span><span class="sxs-lookup"><span data-stu-id="1a697-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="1a697-107">Ändern von DefaultPublicFolderMailbox/EffectivePublicFolderMailbox des Benutzers in ein anderes Postfach als das Inhaltspostfach für den Ordner, der das Problem verursacht</span><span class="sxs-lookup"><span data-stu-id="1a697-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="1a697-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="1a697-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="1a697-109">Warten Sie eine Stunde, und starten Sie den Outlook-Client erneut</span><span class="sxs-lookup"><span data-stu-id="1a697-109">Wait for an hour, restart outlook client</span></span>