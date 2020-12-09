---
title: Automatisches Anmelden bei Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599468"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="7ced6-102">Automatisches Anmelden bei Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="7ced6-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="7ced6-103">Microsoft Edge verwendet das Standardkonto des Betriebssystems, um sich automatisch bei einem Benutzer anzumelden, je nachdem, wie das Gerät des Benutzers konfiguriert ist.</span><span class="sxs-lookup"><span data-stu-id="7ced6-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="7ced6-104">Die Szenarien der einzelnen Geräte Konfigurationstypen und des abhängigen Benutzeranmeldeprozesses werden im folgenden beschrieben:</span><span class="sxs-lookup"><span data-stu-id="7ced6-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="7ced6-105">**Das Gerät ist Hybrid/Aad-J**: diese Option ist unter Windows 10, untergeordnete Fenster und entsprechende Server Versionen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="7ced6-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="7ced6-106">Benutzer werden automatisch mit ihren Azure-Active Directory Konten (AD) angemeldet.</span><span class="sxs-lookup"><span data-stu-id="7ced6-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="7ced6-107">**Das Gerät ist Domänenbeitritt**: diese Option ist unter Windows 10, untergeordnete Fenster und entsprechende Server Versionen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="7ced6-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="7ced6-108">Standardmäßig werden Benutzer mit Domänenkonten nicht automatisch angemeldet; um die automatische Anmeldung für diese zu aktivieren, verwenden Sie die **ConfigureOnPremisesAccountAutoSignIn** -Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="7ced6-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="7ced6-109">Wenn Sie die automatische Anmeldung für Benutzer mit Azure Ad Konten aktivieren möchten, sollten Sie den Hybriden Beitritt zu Ihren Geräten in Frage stellen.</span><span class="sxs-lookup"><span data-stu-id="7ced6-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="7ced6-110">**Das Standardkonto des Betriebssystems ist ein Microsoft-Konto**: diese Option ist unter Windows 10 RS3 (Version 1709, Build 10.0.16299) und höheren Versionen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="7ced6-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="7ced6-111">Das Szenario ist unwahrscheinlich, dass es auf Enterprise-Geräten auftritt.</span><span class="sxs-lookup"><span data-stu-id="7ced6-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="7ced6-112">Wenn das Standardkonto des Betriebssystems jedoch ein Microsoft-Konto ist, meldet sich Microsoft Edge automatisch beim Benutzer mit dem Microsoft-Konto an.</span><span class="sxs-lookup"><span data-stu-id="7ced6-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
