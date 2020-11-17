---
title: Erstellen einer Gruppe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086395"
---
# <a name="create-a-group"></a><span data-ttu-id="b32b1-102">Erstellen einer Gruppe</span><span class="sxs-lookup"><span data-stu-id="b32b1-102">Create a group</span></span>

<span data-ttu-id="b32b1-103">In diesem Thema wird die Gruppenerstellung beschrieben.</span><span class="sxs-lookup"><span data-stu-id="b32b1-103">This topic describes group creation.</span></span>

<span data-ttu-id="b32b1-104">**Berechtigung zum Erstellen einer Gruppe**</span><span class="sxs-lookup"><span data-stu-id="b32b1-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="b32b1-105">Stellen Sie sicher, dass Sie berechtigt sind, eine neue Gruppe zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="b32b1-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="b32b1-106">Globale Administratoren können die Gruppenerstellung im Azure-Portal oder im Access-Bereich deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="b32b1-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="b32b1-107">Möglicherweise benötigen Sie einen Administrator, um die neue Gruppe für Sie zu erstellen oder Ihnen entsprechende Berechtigungen zu erteilen.</span><span class="sxs-lookup"><span data-stu-id="b32b1-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="b32b1-108">**Verwalten von Berechtigungen für die Gruppenerstellung**</span><span class="sxs-lookup"><span data-stu-id="b32b1-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="b32b1-109">Globale Administratoren können Berechtigungen zur Gruppenerstellung (aus Sicherheitsgründen) oder Office 365 Gruppen, die im Azure-Portal oder im Access-Panel erstellt wurden, verwalten, indem Sie "Benutzer können Sicherheitsgruppen in Azure-Portalen erstellen" oder "Benutzer können Office 365 Gruppen in Azure-Portalen erstellen" in **allen Gruppen**  >  **Allgemein (Einstellungen)** auswählen.</span><span class="sxs-lookup"><span data-stu-id="b32b1-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="b32b1-110">Sie können die Gruppenerstellung auch so einschränken, dass eine Gruppe von Benutzern ausgewählt wird, wenn Sie über eine Azure Active Directory P1 Premium-Lizenz verfügen.</span><span class="sxs-lookup"><span data-stu-id="b32b1-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="b32b1-111">**Deaktivieren der Willkommens Benachrichtigung für neue Office 365 Gruppenmitglieder**</span><span class="sxs-lookup"><span data-stu-id="b32b1-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="b32b1-112">Die Willkommens Benachrichtigung, die an Benutzer gesendet wird, die Office 365 Gruppen hinzugefügt werden, kann deaktiviert werden, indem in PowerShell **UnifiedGroupWelcomeMessageEnabled** auf false festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="b32b1-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="b32b1-113">[Hier](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)erfahren Sie mehr über diese Einstellung.</span><span class="sxs-lookup"><span data-stu-id="b32b1-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

