---
title: Microsoft Edge-Support für Microsoft Defender Application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576549"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="47e77-102">Microsoft Edge-Support für Microsoft Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="47e77-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="47e77-103">Entwickelt für Windows 10 und Microsoft Edge verwendet Application Guard einen Ansatz zur Hardware Isolierung, mit dem ein Benutzer eine nicht vertrauenswürdige Website innerhalb eines isolierten Hyper-V-fähigen Containers navigieren kann, der vom Hostbetriebssystem getrennt ist.</span><span class="sxs-lookup"><span data-stu-id="47e77-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="47e77-104">Ein Unternehmensadministrator definiert eine Liste vertrauenswürdiger Websites, Cloud-Ressourcen und interner Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="47e77-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="47e77-105">Wenn ein Benutzer eine Website besucht, die nicht in der Liste enthalten ist, wird die Website von Microsoft Edge im Container geöffnet.</span><span class="sxs-lookup"><span data-stu-id="47e77-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="47e77-106">Dies bedeutet, dass der Host-PC geschützt bleibt und der Angreifer nicht auf die Enterprise-Daten zugreift, wenn die Website als bösartig einstellt wird.</span><span class="sxs-lookup"><span data-stu-id="47e77-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="47e77-107">Die Installation von Erweiterungen im Container wird ab Microsoft Edge Version 81 unterstützt und kann über eine Richtlinie gesteuert werden.</span><span class="sxs-lookup"><span data-stu-id="47e77-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="47e77-108">Die updateURL-Adresse, die in der ExtensionInstallForcelist-Richtlinie verwendet wird, sollte als neutrale Ressource in den vom Application Guard verwendeten Netzwerk Isolierungs Richtlinien hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="47e77-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="47e77-109">Weitere Informationen finden Sie unter [Microsoft Edge Support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="47e77-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
