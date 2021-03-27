---
title: Automatische Anmeldung bei Microsoft Edge
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
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398728"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="4e42e-102">Automatische Anmeldung bei Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="4e42e-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="4e42e-103">Microsoft Edge verwendet das Standardkonto des Betriebssystems, um sich automatisch bei einem Benutzer entsprechend der Konfiguration des Geräts des Benutzers zu anmelden.</span><span class="sxs-lookup"><span data-stu-id="4e42e-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="4e42e-104">Die Szenarien der einzelnen Gerätekonfigurationen und des abhängigen Benutzer-Anmeldevorgangs werden unten beschrieben:</span><span class="sxs-lookup"><span data-stu-id="4e42e-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="4e42e-105">**Das Gerät ist hybrid/AAD-J**: Diese Option ist unter Windows 10, windows-down-level und entsprechenden Serverversionen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="4e42e-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="4e42e-106">Benutzer werden automatisch mit ihren Azure Active Directory (AD)-Konten angemeldet.</span><span class="sxs-lookup"><span data-stu-id="4e42e-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="4e42e-107">**Das Gerät ist mit der Domäne** verbunden: Diese Option ist unter Windows 10, Windows auf down-Level-Ebene und entsprechenden Serverversionen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="4e42e-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="4e42e-108">Standardmäßig werden Benutzer mit Domänenkonten nicht automatisch angemeldet. Verwenden Sie die **ConfigureOnPremisesAccountAutoSignIn-Richtlinie,** um die automatische Anmeldung für sie zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="4e42e-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="4e42e-109">Um die automatische Anmeldung für Benutzer mit Azure AD-Konten zu aktivieren, sollten Sie die Hybridinteging ihrer Geräte in Betracht ziehen.</span><span class="sxs-lookup"><span data-stu-id="4e42e-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="4e42e-110">Das **Standardkonto** des Betriebssystems ist ein Microsoft-Konto: Diese Option ist unter Windows 10 RS3 (Version 1709, Build 10.0.16299) und höher verfügbar.</span><span class="sxs-lookup"><span data-stu-id="4e42e-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="4e42e-111">Das Szenario wird auf Unternehmensgeräten wahrscheinlich nicht auftreten.</span><span class="sxs-lookup"><span data-stu-id="4e42e-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="4e42e-112">Wenn es sich bei dem Standardkonto des Betriebssystems jedoch um ein Microsoft-Konto handelt, wird microsoft Edge den Benutzer automatisch mit dem Microsoft-Konto anmelden.</span><span class="sxs-lookup"><span data-stu-id="4e42e-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
