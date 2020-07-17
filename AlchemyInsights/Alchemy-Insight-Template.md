---
title: identisch mit filename ist am besten
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750969"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="c95a8-102">"Erforderlicher Alchemy-Header H1, H2 funktioniert nicht."</span><span class="sxs-lookup"><span data-stu-id="c95a8-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="c95a8-103">Bewährte Methoden und Richtlinien für die Erstellung von Alchemy-Autoren:</span><span class="sxs-lookup"><span data-stu-id="c95a8-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="c95a8-104">**Alchemy Insights in Folders nicht Schachteln**-dadurch wird die URL-Struktur unterbrochen.</span><span class="sxs-lookup"><span data-stu-id="c95a8-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="c95a8-105">Wir untersuchen, wie Sie dieses Problem beheben.</span><span class="sxs-lookup"><span data-stu-id="c95a8-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="c95a8-106">Dateien im Ordner **AlchemyInsights** sollten klein geschriebene Dateinamen mit Bindestrichen für Leerzeichen (ex) enthalten.</span><span class="sxs-lookup"><span data-stu-id="c95a8-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="c95a8-107">***How-to-enable-Litigation-Hold***.</span><span class="sxs-lookup"><span data-stu-id="c95a8-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="c95a8-108">Schließen Sie die Regel-ID oder Bucket-ID aus dem [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net) in das Feld ms. Custom ein.</span><span class="sxs-lookup"><span data-stu-id="c95a8-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="c95a8-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="c95a8-109">ex.</span></span> <span data-ttu-id="c95a8-110">***ms. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="c95a8-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="c95a8-111">Verwenden Sie die restlichen Metadaten oben in dieser Datei als Vorlage.</span><span class="sxs-lookup"><span data-stu-id="c95a8-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="c95a8-112">Navigieren Sie im [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net)nach unten zum Abschnitt **Kunden Einblicke Title:** , und verwenden Sie diesen als Ausgangspunkt für den H1-Titel für die Einblicke.</span><span class="sxs-lookup"><span data-stu-id="c95a8-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="c95a8-113">Alchemy Insights muss nur ein einzelnes H1 am oberen Rand aufweisen, oder die Produktion wird unterbrochen.</span><span class="sxs-lookup"><span data-stu-id="c95a8-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="c95a8-114">H2s Rendern weder so verwenden Sie **Fett** oder andere Konventionen, um separate Abschnitte zu bedeuten.</span><span class="sxs-lookup"><span data-stu-id="c95a8-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="c95a8-115">Geben Sie als nächstes den Textkörper mithilfe des Entwurfs Materials im Abschnitt Kunden Einblicke der Seite Alchemy Rule ein.</span><span class="sxs-lookup"><span data-stu-id="c95a8-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="c95a8-116">Aufzählungslisten sind in Ordnung</span><span class="sxs-lookup"><span data-stu-id="c95a8-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="c95a8-117">Nummerierte Listen</span><span class="sxs-lookup"><span data-stu-id="c95a8-117">Numbered lists too</span></span>
    1. <span data-ttu-id="c95a8-118">**Fett** und *kursiv* sind a-OK</span><span class="sxs-lookup"><span data-stu-id="c95a8-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="c95a8-119">Links sollten immer entweder **"Links to Internet"/External** oder **Deep-Links zu Benutzeroberflächenelementen**sein, keine internen Links.</span><span class="sxs-lookup"><span data-stu-id="c95a8-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="c95a8-120">Bilder werden zu diesem Zeitpunkt nicht offiziell unterstützt, aber Sie sind in der Roadmap.</span><span class="sxs-lookup"><span data-stu-id="c95a8-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="c95a8-121">Und das ist wirklich schon ein bisschen zu lang.</span><span class="sxs-lookup"><span data-stu-id="c95a8-121">And this is really already a bit too long.</span></span> <span data-ttu-id="c95a8-122">Bewährte Methode sind etwa 400 Zeichen---------------------------------</span><span class="sxs-lookup"><span data-stu-id="c95a8-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="c95a8-123">Nachdem der Inhalt abgeschlossen ist, ziehen Sie ihn in den Live-Zweig.</span><span class="sxs-lookup"><span data-stu-id="c95a8-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="c95a8-124">Wechseln Sie dann zum [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net) , und geben Sie den Dateinamen in das URL-Feld ein.</span><span class="sxs-lookup"><span data-stu-id="c95a8-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 