---
title: Access Services-Ruhestand
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973918"
---
# <a name="access-services-retirement"></a><span data-ttu-id="e4fa8-102">Access Services-Ruhestand</span><span class="sxs-lookup"><span data-stu-id="e4fa8-102">Access services retirement</span></span>

<span data-ttu-id="e4fa8-103">Wie wir ursprünglich in MC97576 angekündigt haben, im März 2017 und weiterhin über das vergangene Jahr kommunizieren, werden Access Services aus Office 365 zurückgezogen.</span><span class="sxs-lookup"><span data-stu-id="e4fa8-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="e4fa8-104">Die nächste Phase dieses Prozesses ist das Entfernen von Access-Webdatenbanken, die SharePoint-Listen als zugrunde liegender Datenspeicher verwenden.</span><span class="sxs-lookup"><span data-stu-id="e4fa8-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

## <a name="how-does-this-affect-me"></a><span data-ttu-id="e4fa8-105">Wie wirkt sich das auf mich aus?</span><span class="sxs-lookup"><span data-stu-id="e4fa8-105">How does this affect me?</span></span>

<span data-ttu-id="e4fa8-106">Ab Juni 2019 werden wir die Erstellung neuer Access-Datenbanken in SharePoint Online beenden und den Dienst und alle verbleibenden apps bis April 2020 Herunterfahren.</span><span class="sxs-lookup"><span data-stu-id="e4fa8-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a><span data-ttu-id="e4fa8-107">Was muss ich tun, um diese Änderung vorzubereiten?</span><span class="sxs-lookup"><span data-stu-id="e4fa8-107">What do I need to do to prepare for this change?</span></span>

<span data-ttu-id="e4fa8-108">Wir empfehlen Ihnen, einen Übergangsplan für die Access-Webdatenbanken Ihrer Organisation zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="e4fa8-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="e4fa8-109">Administratoren können den [SharePoint Access-App-Scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) verwenden, um eine Bestandsaufnahme der Access-apps abzurufen, die von Websites verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="e4fa8-109">Admins can use the [SharePoint Access app scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="e4fa8-110">Es gibt mehrere Möglichkeiten zum Migrieren von Daten in Access-Webdatenbanken:</span><span class="sxs-lookup"><span data-stu-id="e4fa8-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="e4fa8-111">Importieren in eine lokale Access-Datenbank (. ACCDB) oder in eine Excel-Datei.</span><span class="sxs-lookup"><span data-stu-id="e4fa8-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="e4fa8-112">Außerdem wird empfohlen, Microsoft PowerApps als Alternative Plattform für die Erstellung von Unternehmenslösungen ohne Code für Web-und mobile Geräte zu erkunden.</span><span class="sxs-lookup"><span data-stu-id="e4fa8-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>