---
title: Tauschen Sie Ihre klassische Stammwebsite mit einer modernen Website aus.
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36749259"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="790ef-102">Tauschen Sie Ihre klassische Stammwebsite mit einer modernen Website aus.</span><span class="sxs-lookup"><span data-stu-id="790ef-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="790ef-103">Wenn Ihre Umgebung vor dem 2019 April eingerichtet wurde, können Sie die Stammwebsite mithilfe von Microsoft PowerShell in eine moderne Website ändern:</span><span class="sxs-lookup"><span data-stu-id="790ef-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="790ef-104">Wenn Sie eine andere Website als Stammwebsite verwenden möchten, können Sie die Stammwebsite durch diese ersetzen [(tauschen)](https://docs.microsoft.com/sharepoint/modern-root-site) .</span><span class="sxs-lookup"><span data-stu-id="790ef-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="790ef-105">Verwenden Sie [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , um den Speicherort einer Website während der Archivierung der ursprünglichen Website mit einer anderen Website zu vertauschen.</span><span class="sxs-lookup"><span data-stu-id="790ef-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="790ef-106">Für beide Team Websites (nicht verbunden mit einer Gruppe) und Kommunikationswebsite verfügbar.</span><span class="sxs-lookup"><span data-stu-id="790ef-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="790ef-107">In Kürze werden zusätzliche Funktionen eingeführt, mit denen Sie die Inhalte auf der Website weiterhin verwenden, die vorhandene Website jedoch in eine Kommunikationswebsite umwandeln können.</span><span class="sxs-lookup"><span data-stu-id="790ef-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="790ef-108">Diese Funktionen werden schrittweise ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="790ef-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="790ef-109">Fahren Sie mit dem Überprüfen des Office 365 Nachrichten Centers auf Updates fort.</span><span class="sxs-lookup"><span data-stu-id="790ef-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="790ef-110">Bekannte Probleme beim Austauschen von Websites</span><span class="sxs-lookup"><span data-stu-id="790ef-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="790ef-111">Die Zielwebsite gibt möglicherweise einen Fehler "nicht gefunden" (HTTP 404) für eine kurze Zeit zurück.</span><span class="sxs-lookup"><span data-stu-id="790ef-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="790ef-112">Der Inhalt muss erneut durchforstet werden, um den Suchindex zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="790ef-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="790ef-113">Es ist kein manueller Schritt erforderlich – Dies erfolgt automatisch.</span><span class="sxs-lookup"><span data-stu-id="790ef-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="790ef-114">Alles, was von "statischen" Links (wie Dateisynchronisierung und OneNote-Dateien) abhängig ist, muss manuell korrigiert werden.</span><span class="sxs-lookup"><span data-stu-id="790ef-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="790ef-115">Wenn es sich bei der Quellwebsite um eine organisatorische Nachrichtenwebsite handelt, aktualisieren Sie die URL.</span><span class="sxs-lookup"><span data-stu-id="790ef-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="790ef-116">Hier erhalten Sie eine Liste aller Nachrichtenwebsites für die Organisation.</span><span class="sxs-lookup"><span data-stu-id="790ef-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="790ef-117">Project Server-Websites müssen möglicherweise überprüft werden, um sicherzustellen, dass Sie weiterhin ordnungsgemäß zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="790ef-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





