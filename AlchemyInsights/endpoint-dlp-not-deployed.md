---
title: Verhinderung von Datenverlust am Endpunkt auf dem Gerät des Benutzers nicht bereitgestellt
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/27/2021
ms.locfileid: "52694806"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="a77d4-102">Verhinderung von Datenverlust am Endpunkt auf dem Gerät des Benutzers nicht bereitgestellt</span><span class="sxs-lookup"><span data-stu-id="a77d4-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="a77d4-103">Wenn die Einstellung für die Verhinderung von Datenverlust am Endpunkt nicht auf das Gerät eines Benutzers angewendet wurde, stellen Sie sicher, dass Sie die folgenden Kriterien erfüllt sind:</span><span class="sxs-lookup"><span data-stu-id="a77d4-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="a77d4-104">Auf dem Gerät ist Windows 10 x64, Build 1809 oder höher, installiert.</span><span class="sxs-lookup"><span data-stu-id="a77d4-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="a77d4-105">Antischadsoftware-Client, Version 4.18.2009.7 oder höher, ist installiert.</span><span class="sxs-lookup"><span data-stu-id="a77d4-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="a77d4-106">Auf das Gerät trifft **einer** der folgenden Punkte zu:</span><span class="sxs-lookup"><span data-stu-id="a77d4-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="a77d4-107">Es ist in Azure Active Directory (Azure AD) eingebunden</span><span class="sxs-lookup"><span data-stu-id="a77d4-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="a77d4-108">Es ist in Azure AD Hybrid eingebunden</span><span class="sxs-lookup"><span data-stu-id="a77d4-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="a77d4-109">Es ist in AAD registriert</span><span class="sxs-lookup"><span data-stu-id="a77d4-109">AAD registered</span></span>

- <span data-ttu-id="a77d4-110">Um Richtlinienaktionen durchzusetzen, stellen Sie sicher, dass der Microsoft Chromium Edge-Browser auf dem Endpunktgerät installiert ist.</span><span class="sxs-lookup"><span data-stu-id="a77d4-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="a77d4-111">Weitere Anforderungen für die Bereitstellung der Verhinderung von Datenverlust am Endpunkt finden Sie unter [Erste Schritte mit der Verhinderung von Datenverlust am Endpunkt](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span><span class="sxs-lookup"><span data-stu-id="a77d4-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>