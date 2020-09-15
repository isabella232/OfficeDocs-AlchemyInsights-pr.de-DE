---
title: Ruhestand "Access Services"
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698681"
---
# <a name="access-services-retirement"></a><span data-ttu-id="3eae2-102">Ruhestand "Access Services"</span><span class="sxs-lookup"><span data-stu-id="3eae2-102">Access services retirement</span></span>

<span data-ttu-id="3eae2-103">Wie wir ursprünglich in MC97576 angekündigt haben, im März 2017, und weiterhin im vergangenen Jahr kommuniziert haben Access Services werden ausgemustert.</span><span class="sxs-lookup"><span data-stu-id="3eae2-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="3eae2-104">Die nächste Phase in diesem Prozess wird das Entfernen von Access-Webdatenbanken sein, die SharePoint-Listen als zugrunde liegender Datenspeicher verwenden.</span><span class="sxs-lookup"><span data-stu-id="3eae2-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="3eae2-105">**Wie wirkt sich dies auf mich aus?**</span><span class="sxs-lookup"><span data-stu-id="3eae2-105">**How does this affect me?**</span></span>

<span data-ttu-id="3eae2-106">Ab Juni 2019 werden wir die Erstellung neuer Access-Datenbanken in SharePoint Online beenden und den Dienst und alle verbleibenden apps bis April 2020 Herunterfahren.</span><span class="sxs-lookup"><span data-stu-id="3eae2-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="3eae2-107">**Was muss ich tun, um diese Änderung vorzubereiten?**</span><span class="sxs-lookup"><span data-stu-id="3eae2-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="3eae2-108">Wir empfehlen Ihnen, einen Übergangsplan für die Access-Webdatenbanken Ihrer Organisation zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="3eae2-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="3eae2-109">Administratoren können den [SharePoint Access-App-Scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) verwenden, um eine Bestandsaufnahme der Access-apps zu erhalten, die von Websites verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="3eae2-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="3eae2-110">Es gibt verschiedene Möglichkeiten zum Migrieren von Access-Daten Bank Datenbanken:</span><span class="sxs-lookup"><span data-stu-id="3eae2-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="3eae2-111">Importieren in eine lokale Access-Datenbank (. ACCDB) oder in eine Excel-Datei.</span><span class="sxs-lookup"><span data-stu-id="3eae2-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="3eae2-112">Außerdem wird empfohlen, Microsoft PowerApps als Alternative Plattform zum Erstellen von codelosen Geschäftslösungen für das Internet und mobile Geräte zu erforschen.</span><span class="sxs-lookup"><span data-stu-id="3eae2-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>