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
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="bcd2a-102">Besitzer kann keinen Unterordner mit Outlook erstellen</span><span class="sxs-lookup"><span data-stu-id="bcd2a-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="bcd2a-103">**Es gibt ein anhaltendes Problem mit Besitzern öffentlicher Ordner, die Unterordner mit Outlook erstellen. Das Problem wird in Kürze behoben.**</span><span class="sxs-lookup"><span data-stu-id="bcd2a-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="bcd2a-104">In der Zwischenzeit können Sie eine der folgenden Problemumgehungen verwenden:</span><span class="sxs-lookup"><span data-stu-id="bcd2a-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="bcd2a-105">Verwenden Sie Outlook für MAC, um den Unterordner zu erstellen, da das Problem nur Outlook für Desktop-Fenster betrifft (alle Versionen)</span><span class="sxs-lookup"><span data-stu-id="bcd2a-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="bcd2a-106">Lassen Sie den Administrator den Unterordner mit EXO Shell oder EAC erstellen</span><span class="sxs-lookup"><span data-stu-id="bcd2a-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="bcd2a-107">Ändern von DefaultPublicFolderMailbox/EffectivePublicFolderMailbox des Benutzers in ein anderes Postfach als das Inhaltspostfach für den Ordner, der das Problem verursacht</span><span class="sxs-lookup"><span data-stu-id="bcd2a-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="bcd2a-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="bcd2a-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="bcd2a-109">Warten Sie eine Stunde, und starten Sie den Outlook-Client erneut</span><span class="sxs-lookup"><span data-stu-id="bcd2a-109">Wait for an hour, restart outlook client</span></span>