---
title: Informationen zur Identität in Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664169"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="07a96-102">Informationen zur Identität in Yammer</span><span class="sxs-lookup"><span data-stu-id="07a96-102">About identity in Yammer</span></span>

<span data-ttu-id="07a96-103">Es wird empfohlen, dass für alle Netzwerke die folgenden Schritte ausgeführt werden, um identitätsbezogene Probleme zu vermeiden:</span><span class="sxs-lookup"><span data-stu-id="07a96-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="07a96-104">Erzwingen Sie die Office 365-Identität nach der Bereitstellung von Microsoft 365-Konten für Benutzer in Azure AD, um sicherzustellen, dass alle Benutzer sich mit ihrem Microsoft 365-Hauptkonto anmelden.</span><span class="sxs-lookup"><span data-stu-id="07a96-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="07a96-105">Weitere Informationen finden Sie unter [Erzwingen der Office 365-Identität für Yammer-Benutzer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="07a96-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="07a96-106">Konsolidieren Sie mehrerer Yammer-Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="07a96-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="07a96-107">Älteren Yammer-Konfigurationen erlauben, dass mehrere Yammer-Netzwerke mit einem Mandanten verbunden werden.</span><span class="sxs-lookup"><span data-stu-id="07a96-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="07a96-108">Weitere Informationen finden Sie unter [Netzwerkmigration: Konsolidieren von mehreren Yammer-Netzwerken](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="07a96-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="07a96-109">Optional können Sie eine Lizenz für Yammer erzwingen, um die Verwendung von Yammer für Benutzer ohne Lizenz zu sperren.</span><span class="sxs-lookup"><span data-stu-id="07a96-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="07a96-110">Weitere Informationen finden Sie unter [Verwalten von Yammer-Benutzerlizenzen in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="07a96-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="07a96-111">Überprüfen Sie abschließend die Benutzerliste für ältere Yammer-Netzwerke, und sperren Sie Legacybenutzer.</span><span class="sxs-lookup"><span data-stu-id="07a96-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="07a96-112">Es wird empfohlen, die Benutzer auszusetzen (zu deaktivieren), statt sie zu löschen, da das Löschen nicht rückgängig gemacht werden kann.</span><span class="sxs-lookup"><span data-stu-id="07a96-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="07a96-113">Weitere Informationen finden Sie unter [Überwachen von Yammer-Benutzern in mit Office 365 verbundenen Netzwerken](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) und [Entfernen von Benutzern](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="07a96-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="07a96-114">Indem Sie Yammer mit diesen Schritten konfigurieren, sind Sie auch bereit, Ihr Yammer Netzwerk für Microsoft 365 für den nativen Modus zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="07a96-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="07a96-115">Weitere Informationen finden Sie unter [Konfigurieren eines Yammer-Netzwerks für den nativen Modus für Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="07a96-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>