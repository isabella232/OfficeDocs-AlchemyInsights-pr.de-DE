---
title: 'identisch mit filename ist am besten [RULE #-Description]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634503"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="732c4-102">Erforderlicher Alchemy-Header H1, H2 funktioniert nicht.</span><span class="sxs-lookup"><span data-stu-id="732c4-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="732c4-103">Bewährte Methoden und Richtlinien für die Erstellung von Alchemie:</span><span class="sxs-lookup"><span data-stu-id="732c4-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="732c4-104">**Verschachteln Sie Alchemy Insights nicht in Ordnern**– dadurch wird die URL-Struktur unterbrochen.</span><span class="sxs-lookup"><span data-stu-id="732c4-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="732c4-105">Wir untersuchen, dies zu beheben.</span><span class="sxs-lookup"><span data-stu-id="732c4-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="732c4-106">Dateien im Ordner **AlchemyInsights** sollten über das [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net) im Dateinamen Regel-ID und Regelname enthalten.</span><span class="sxs-lookup"><span data-stu-id="732c4-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="732c4-107">Ex.</span><span class="sxs-lookup"><span data-stu-id="732c4-107">ex.</span></span> <span data-ttu-id="732c4-108">***976-enable-Litigation-Hold***</span><span class="sxs-lookup"><span data-stu-id="732c4-108">***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="732c4-109">Verwenden Sie die Metadaten am Anfang dieser Datei als Vorlage.</span><span class="sxs-lookup"><span data-stu-id="732c4-109">Use the metadata at the top of this file as your template.</span></span> <span data-ttu-id="732c4-110">Es ist nichts anderes erforderlich.</span><span class="sxs-lookup"><span data-stu-id="732c4-110">Nothing else is required.</span></span>
1. <span data-ttu-id="732c4-111">Navigieren Sie im [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net)zum Abschnitt **Customer Insight Title:** und verwenden Sie diesen als Ausgangspunkt für Ihren H1-Titel für die Einblicke.</span><span class="sxs-lookup"><span data-stu-id="732c4-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="732c4-112">Alchemy inSights muss oben nur einen einzelnen H1 haben, oder Sie werden in der Produktion unterbrochen.</span><span class="sxs-lookup"><span data-stu-id="732c4-112">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="732c4-113">H2s nicht rendern, verwenden Sie daher **Fett** oder andere Konventionen, um separate Abschnitte anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="732c4-113">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="732c4-114">Als nächstes füllen Sie den Textkörper mit dem Entwurfsmaterial im Abschnitt Kunden einBlicke auf der Seite Alchemy Rule aus.</span><span class="sxs-lookup"><span data-stu-id="732c4-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="732c4-115">AufZählungslisten sind in Ordnung</span><span class="sxs-lookup"><span data-stu-id="732c4-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="732c4-116">Nummerierte Listen</span><span class="sxs-lookup"><span data-stu-id="732c4-116">Numbered lists too</span></span>
    1. <span data-ttu-id="732c4-117">**Fett** und *kursiv* sind a-OK</span><span class="sxs-lookup"><span data-stu-id="732c4-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="732c4-118">Links sollten immer entweder **"Links zu Web"/External** oder **Deep-Links zu UI-Elementen**, nicht interne Links.</span><span class="sxs-lookup"><span data-stu-id="732c4-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="732c4-119">Und das ist wirklich schon ein bisschen zu lang.</span><span class="sxs-lookup"><span data-stu-id="732c4-119">And this is really already a bit too long.</span></span> <span data-ttu-id="732c4-120">Die bewährte Methode umfasst ungefähr 400 Zeichen---------------------------------</span><span class="sxs-lookup"><span data-stu-id="732c4-120">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="732c4-121">Sobald Ihr Inhalt fertig ist, ziehen Sie ihn in die Live-Verzweigung.</span><span class="sxs-lookup"><span data-stu-id="732c4-121">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="732c4-122">Wechseln Sie dann zum [Alchemy-Partner Portal](https://alchemyportal.azurewebsites.net) , und geben Sie den Dateinamen in das Feld URL ein.</span><span class="sxs-lookup"><span data-stu-id="732c4-122">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="732c4-123">Vergewissern Sie sich, dass einBlicke überprüft und veröffentlicht werden, und klicken Sie auf Regel aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="732c4-123">Make sure Insight reviewed and published says "yes" and then click Update Rule.</span></span> <span data-ttu-id="732c4-124">**(Dies wird in der neuen Version des Portals schöner aussehen-Veröffentlichung in Kürze.)** 
 ![](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="732c4-124">**(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

