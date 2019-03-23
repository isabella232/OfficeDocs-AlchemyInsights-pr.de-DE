---
title: identisch mit filename am besten
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 37398436435fb72cb5c8dca2d0798b86a0c8ccc9
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/22/2019
ms.locfileid: "30762064"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="cb537-102">Erforderlicher Alchemy-Header H1, H2 funktioniert nicht.</span><span class="sxs-lookup"><span data-stu-id="cb537-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="cb537-103">Bewährte Methoden und Richtlinien für die Erstellung von Alchemie:</span><span class="sxs-lookup"><span data-stu-id="cb537-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="cb537-104">**Verschachteln Sie Alchemy Insights nicht in Ordnern**– dadurch wird die URL-Struktur unterbrochen.</span><span class="sxs-lookup"><span data-stu-id="cb537-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="cb537-105">Wir untersuchen, dies zu beheben.</span><span class="sxs-lookup"><span data-stu-id="cb537-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="cb537-106">Dateien im Ordner **AlchemyInsights** sollten Kleinbuchstaben-Dateinamen mit Bindestrichen für Leerzeichen enthalten.</span><span class="sxs-lookup"><span data-stu-id="cb537-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="cb537-107">***How-to-enable-Litigation-Hold***.</span><span class="sxs-lookup"><span data-stu-id="cb537-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="cb537-108">Schließen Sie die Regel-ID oder die Bucket-ID aus dem [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net) in das Feld ms. Custom ein.</span><span class="sxs-lookup"><span data-stu-id="cb537-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="cb537-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="cb537-109">ex.</span></span> <span data-ttu-id="cb537-110">***ms. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="cb537-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="cb537-111">Verwenden Sie die restlichen Metadaten am Anfang dieser Datei als Vorlage.</span><span class="sxs-lookup"><span data-stu-id="cb537-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="cb537-112">Navigieren Sie im [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net)zum Abschnitt **Customer Insight Title:** und verwenden Sie diesen als Ausgangspunkt für Ihren H1-Titel für die Einblicke.</span><span class="sxs-lookup"><span data-stu-id="cb537-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="cb537-113">Alchemy inSights muss oben nur einen einzelnen H1 haben, oder Sie werden in der Produktion unterbrochen.</span><span class="sxs-lookup"><span data-stu-id="cb537-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="cb537-114">H2s nicht rendern, verwenden Sie daher **Fett** oder andere Konventionen, um separate Abschnitte anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="cb537-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="cb537-115">Als nächstes füllen Sie den Textkörper mit dem Entwurfsmaterial im Abschnitt Kunden einBlicke auf der Seite Alchemy Rule aus.</span><span class="sxs-lookup"><span data-stu-id="cb537-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="cb537-116">AufZählungslisten sind in Ordnung</span><span class="sxs-lookup"><span data-stu-id="cb537-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="cb537-117">Nummerierte Listen</span><span class="sxs-lookup"><span data-stu-id="cb537-117">Numbered lists too</span></span>
    1. <span data-ttu-id="cb537-118">**Fett** und *kursiv* sind a-OK</span><span class="sxs-lookup"><span data-stu-id="cb537-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="cb537-119">Links sollten immer entweder **"Links zu Web"/External** oder **Deep-Links zu UI-Elementen**, nicht interne Links.</span><span class="sxs-lookup"><span data-stu-id="cb537-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="cb537-120">Bilder werden zu diesem Zeitpunkt nicht offiziell unterstützt, aber es steht in der Roadmap.</span><span class="sxs-lookup"><span data-stu-id="cb537-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="cb537-121">Und das ist wirklich schon ein bisschen zu lang.</span><span class="sxs-lookup"><span data-stu-id="cb537-121">And this is really already a bit too long.</span></span> <span data-ttu-id="cb537-122">Die bewährte Methode umfasst ungefähr 400 Zeichen---------------------------------</span><span class="sxs-lookup"><span data-stu-id="cb537-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="cb537-123">Sobald Ihr Inhalt fertig ist, ziehen Sie ihn in die Live-Verzweigung.</span><span class="sxs-lookup"><span data-stu-id="cb537-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="cb537-124">Wechseln Sie dann zum [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net) , und geben Sie den Dateinamen in das Feld URL ein.</span><span class="sxs-lookup"><span data-stu-id="cb537-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="cb537-125">M</span><span class="sxs-lookup"><span data-stu-id="cb537-125">M</span></span>