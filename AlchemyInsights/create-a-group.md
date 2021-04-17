---
title: Erstellen einer Gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816355"
---
# <a name="create-a-group"></a><span data-ttu-id="dd1cc-102">Erstellen einer Gruppe</span><span class="sxs-lookup"><span data-stu-id="dd1cc-102">Create a group</span></span>

<span data-ttu-id="dd1cc-103">In diesem Thema wird die Gruppenerstellung beschrieben.</span><span class="sxs-lookup"><span data-stu-id="dd1cc-103">This topic describes group creation.</span></span>

<span data-ttu-id="dd1cc-104">**Berechtigung zum Erstellen einer Gruppe**</span><span class="sxs-lookup"><span data-stu-id="dd1cc-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="dd1cc-105">Stellen Sie sicher, dass Sie autorisiert sind, eine neue Gruppe zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="dd1cc-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="dd1cc-106">Globale Administratoren können die Gruppenerstellung im Microsoft Azure-Portal oder im Access Panel deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="dd1cc-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="dd1cc-107">Möglicherweise benötigen Sie einen Administrator, um die neue Gruppe für Sie zu erstellen oder Ihnen die entsprechenden Berechtigungen zu erteilen.</span><span class="sxs-lookup"><span data-stu-id="dd1cc-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="dd1cc-108">**Verwalten von Gruppenerstellungsberechtigungen**</span><span class="sxs-lookup"><span data-stu-id="dd1cc-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="dd1cc-109">Globale Administratoren können Gruppenerstellungsberechtigungen (aus sicherheitsbezogenen Gründen) oder Office 365-Gruppen verwalten, die im Azure-Portal oder im Zugriffsbereich erstellt wurden, indem sie unter **Alle** Gruppen  >  **Allgemein (Einstellungen)** die Optionen "Benutzer können Sicherheitsgruppen in Azure-Portalen erstellen" oder "Benutzer können Office 365-Gruppen in Azure-Portalen erstellen" auswählen.</span><span class="sxs-lookup"><span data-stu-id="dd1cc-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="dd1cc-110">Sie können die Gruppenerstellung auch einschränken, um eine Gruppe von Benutzern auszuwählen, wenn Sie über eine Azure Active Directory P1 Premium-Lizenz verfügen.</span><span class="sxs-lookup"><span data-stu-id="dd1cc-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="dd1cc-111">**Deaktivieren der Willkommensbenachrichtigung für neue Office 365-Gruppenmitglieder**</span><span class="sxs-lookup"><span data-stu-id="dd1cc-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="dd1cc-112">Die Willkommensbenachrichtigung, die an Benutzer gesendet wird, die Office 365-Gruppen hinzugefügt werden, kann deaktiviert werden, indem **UnifiedGroupWelcomeMessageEnabled** in Powershell auf False gesetzt wird.</span><span class="sxs-lookup"><span data-stu-id="dd1cc-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="dd1cc-113">Erfahren Sie [hier](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true) mehr über diese Einstellung.</span><span class="sxs-lookup"><span data-stu-id="dd1cc-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

