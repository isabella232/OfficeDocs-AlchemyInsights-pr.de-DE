---
title: Website oder Liste als Vorlage speichern
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 627f49991aaef984f731412045351d7a1862b376
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048723"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="853fe-102">Website oder Liste als Vorlage speichern</span><span class="sxs-lookup"><span data-stu-id="853fe-102">Save site or list as a template</span></span>

<span data-ttu-id="853fe-103">SharePoint-Websitevorlagen sind vorkonfigurierte Definitionen, die einem bestimmten Geschäftszweck dienen.</span><span class="sxs-lookup"><span data-stu-id="853fe-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="853fe-104">Weitere Informationen finden Sie unter [Verwenden von Vorlagen zum Erstellen unterschiedlicher Arten von SharePoint-Websites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="853fe-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="853fe-105">Im folgenden finden Sie einige häufige Probleme/Lösungen zum Speichern einer Website oder Liste als Vorlage in SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="853fe-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="853fe-106">**Die Schaltfläche Website/Listenvorlage speichern ist nicht verfügbar oder fehlt**.</span><span class="sxs-lookup"><span data-stu-id="853fe-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="853fe-107">Administratoren müssen benutzerdefiniertes Skript zulassen, um die Vorlagen Features zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="853fe-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="853fe-108">Ausführliche Schritte, Beispiele und Überlegungen finden Sie unter [zulassen oder verhindern von benutzerdefiniertem Skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="853fe-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="853fe-109">Der Befehl Website als Vorlage speichern wird nicht unterstützt und kann Probleme auf Websites mit der SharePoint Server Veröffentlichungs Infrastruktur verursachen.</span><span class="sxs-lookup"><span data-stu-id="853fe-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="853fe-110">**Die Websitevorlage kann nicht erstellt werden oder funktioniert nicht ordnungsgemäß.**</span><span class="sxs-lookup"><span data-stu-id="853fe-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="853fe-111">Die Vorlage fehlt möglicherweise ein [Feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) und wird nicht aktiviert.</span><span class="sxs-lookup"><span data-stu-id="853fe-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="853fe-112">Wenn das Feature nicht zur Aktivierung in der aktuellen Websitesammlung verfügbar ist, können Sie die Websitevorlage nicht zum Erstellen einer Website verwenden.</span><span class="sxs-lookup"><span data-stu-id="853fe-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="853fe-113">Überprüfen Sie, ob Listen oder Bibliotheken den Grenzwert für die [Listenansicht](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) von 5000 Elementen überschreiten, da dadurch das Erstellen einer Websitevorlage blockiert werden kann.</span><span class="sxs-lookup"><span data-stu-id="853fe-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="853fe-114">Die Website verwendet möglicherweise zu viele Ressourcen, und daher überschreitet die Websitevorlage den Grenzwert von 50 MB.</span><span class="sxs-lookup"><span data-stu-id="853fe-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="853fe-115">Es gibt Probleme beim Anzeigen von Daten aus einer Liste, die eine Nachschlagespalte verwendet.</span><span class="sxs-lookup"><span data-stu-id="853fe-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="853fe-116">Weitere Informationen finden Sie unter [Template-generated list zeigt keine Daten aus der richtigen Nachschlageliste in SharePoint Online an](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="853fe-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="853fe-117">Ausführlichere Informationen zu häufig auftretenden Problemen und Lösungen finden Sie unter Referenz, [Erstellen und Verwenden von Websitevorlagen](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="853fe-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

