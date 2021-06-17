---
title: Verwenden von Microsoft Intune zum Verwalten des Webzugriffs in Microsoft Edge für iOS und Android
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989672"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="c5cbd-102">Verwenden von Microsoft Intune zum Verwalten des Webzugriffs in Microsoft Edge für iOS und Android</span><span class="sxs-lookup"><span data-stu-id="c5cbd-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="c5cbd-103">Microsoft Edge für iOS und Android können Benutzer das Web aus mehreren, vollständig getrennten Profilen durchsuchen.</span><span class="sxs-lookup"><span data-stu-id="c5cbd-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="c5cbd-104">Die umfassendsten Schutzfunktionen für Microsoft 365 Daten werden verfügbar, wenn Sie die Enterprise Mobility + Security-Suite abonnieren, die Microsoft Intune und Azure Active Directory Premium Features wie bedingten Zugriff umfasst.</span><span class="sxs-lookup"><span data-stu-id="c5cbd-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="c5cbd-105">Sie sollten mindestens eine Richtlinie für bedingten Zugriff bereitstellen, mit der (1) Benutzer eine Verbindung von mobilen Geräten mit Microsoft Edge für iOS und Android herstellen können und die (2) eine Microsoft Intune App-Schutzrichtlinie implementiert, die eine geschützte Browserumgebung bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="c5cbd-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="c5cbd-106">Informationen dazu, wie Sie bedingten Zugriff und Richtlinien verwenden können, finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="c5cbd-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="c5cbd-107">Anwenden Azure Active Directory Richtlinien für bedingten Zugriff</span><span class="sxs-lookup"><span data-stu-id="c5cbd-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="c5cbd-108">Erstellen Microsoft Intune App-Schutzrichtlinien</span><span class="sxs-lookup"><span data-stu-id="c5cbd-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="c5cbd-109">Verwenden des einmaligen Anmeldens für Azure Active Directory-verbundene Web-Apps in richtliniengeschützten Browsern</span><span class="sxs-lookup"><span data-stu-id="c5cbd-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="c5cbd-110">Verwenden der App-Konfiguration zum Verwalten der Browserumgebung</span><span class="sxs-lookup"><span data-stu-id="c5cbd-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="c5cbd-111">Ausschließliche Verwendung von Geschäfts-, Schul- und Unikonten zulassen</span><span class="sxs-lookup"><span data-stu-id="c5cbd-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="c5cbd-112">Bereitstellen allgemeiner App-Konfigurationsrichtlinien</span><span class="sxs-lookup"><span data-stu-id="c5cbd-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="c5cbd-113">Bereitstellen von App-Konfigurationsrichtlinien für den Datenschutz</span><span class="sxs-lookup"><span data-stu-id="c5cbd-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="c5cbd-114">Verwenden von Microsoft Endpoint Manager zum Bereitstellen von App-Konfigurationsrichtlinien</span><span class="sxs-lookup"><span data-stu-id="c5cbd-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="c5cbd-115">Informationen zum Zugreifen auf Protokolle verwalteter Apps finden Sie unter [Verwenden von Microsoft Edge für iOS und Android, um auf Protokolle verwalteter Apps zuzugreifen.](https://go.microsoft.com/fwlink/?linkid=2132578)</span><span class="sxs-lookup"><span data-stu-id="c5cbd-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
