---
title: Ruhestand "Access Services"
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36747783"
---
# <a name="access-services-retirement"></a><span data-ttu-id="603e8-102">Ruhestand "Access Services"</span><span class="sxs-lookup"><span data-stu-id="603e8-102">Access services retirement</span></span>

<span data-ttu-id="603e8-103">Wie wir ursprünglich in MC97576 angekündigt haben, im März 2017 und im vergangenen Jahr weiter kommuniziert haben, werden Access Services von Office 365 zurückgezogen.</span><span class="sxs-lookup"><span data-stu-id="603e8-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="603e8-104">Die nächste Phase in diesem Prozess wird das Entfernen von Access-Webdatenbanken sein, die SharePoint-Listen als zugrunde liegender Datenspeicher verwenden.</span><span class="sxs-lookup"><span data-stu-id="603e8-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="603e8-105">**Wie wirkt sich dies auf mich aus?**</span><span class="sxs-lookup"><span data-stu-id="603e8-105">**How does this affect me?**</span></span>

<span data-ttu-id="603e8-106">Ab Juni 2019 werden wir die Erstellung neuer Access-Datenbanken in SharePoint Online beenden und den Dienst und alle verbleibenden apps bis April 2020 Herunterfahren.</span><span class="sxs-lookup"><span data-stu-id="603e8-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="603e8-107">**Was muss ich tun, um diese Änderung vorzubereiten?**</span><span class="sxs-lookup"><span data-stu-id="603e8-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="603e8-108">Wir empfehlen Ihnen, einen Übergangsplan für die Access-Webdatenbanken Ihrer Organisation zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="603e8-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="603e8-109">Administratoren können den [SharePoint Access-App-Scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) verwenden, um eine Bestandsaufnahme der Access-apps zu erhalten, die von Websites verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="603e8-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="603e8-110">Es gibt verschiedene Möglichkeiten zum Migrieren von Access-Daten Bank Datenbanken:</span><span class="sxs-lookup"><span data-stu-id="603e8-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="603e8-111">Importieren in eine lokale Access-Datenbank (. ACCDB) oder in eine Excel-Datei.</span><span class="sxs-lookup"><span data-stu-id="603e8-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="603e8-112">Außerdem wird empfohlen, Microsoft PowerApps als Alternative Plattform zum Erstellen von codelosen Geschäftslösungen für das Internet und mobile Geräte zu erforschen.</span><span class="sxs-lookup"><span data-stu-id="603e8-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>