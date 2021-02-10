---
title: Problem mit Sicherheitsgruppen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162926"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="66c27-102">Problem mit Sicherheitsgruppen</span><span class="sxs-lookup"><span data-stu-id="66c27-102">Issue with security groups</span></span>

<span data-ttu-id="66c27-103">**Wenn Sie Netzwerkfehler des Typs AADDS104 erhalten**</span><span class="sxs-lookup"><span data-stu-id="66c27-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="66c27-104">Ungültige Regeln für Netzwerksicherheitsgruppen sind die häufigste Ursache für Netzwerkfehler in Azure Active Directory Domain Services (AD DS).</span><span class="sxs-lookup"><span data-stu-id="66c27-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="66c27-105">Die Netzwerksicherheitsgruppe für das virtuelle Netzwerk muss den Zugriff auf bestimmte Ports und Protokolle zulassen.</span><span class="sxs-lookup"><span data-stu-id="66c27-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="66c27-106">Wenn diese Ports blockiert sind, kann die Azure-Plattform die verwaltete Domäne nicht überwachen oder aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="66c27-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="66c27-107">Die Synchronisierung zwischen Azure AD und Azure AD DS ist ebenfalls betroffen.</span><span class="sxs-lookup"><span data-stu-id="66c27-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="66c27-108">Stellen Sie sicher, dass die Standardports geöffnet bleiben, um Dienstunterbrechungen zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="66c27-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="66c27-109">Informationen zum Verstehen und Beheben häufiger Warnungen zu Konfigurationsproblemen bei der Netzwerksicherheitsgruppe finden Sie unter [Hinzufügen und Überprüfen von Sicherheitsgruppen](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span><span class="sxs-lookup"><span data-stu-id="66c27-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
