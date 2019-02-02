---
title: identisch mit Filename am besten geeignet ist [Regel c#-Beschreibung]
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 278a26f4b986a85e33442baef690d3bb44462ace
ms.sourcegitcommit: 32355b76d45b730a069575efeec708149d4aeaa3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/01/2019
ms.locfileid: "29697129"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="69ce7-102">Erforderliche Alchemy Kopfzeile H1, H2 des funktionieren nicht.</span><span class="sxs-lookup"><span data-stu-id="69ce7-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="69ce7-103">Bewährte Methoden und Richtlinien zum Erstellen von Alchemy:</span><span class="sxs-lookup"><span data-stu-id="69ce7-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="69ce7-p101">**Alchemy Einblicke in Ordnern nicht schachteln**- Url-Struktur umbrochen werden. Wir versuchen beheben.</span><span class="sxs-lookup"><span data-stu-id="69ce7-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="69ce7-106">Dateien im Ordner **AlchemyInsights** sollte Regel-ID und Name der Regel über das [Portal Alchemy Partner](https://alchemyportal.azurewebsites.net) im Dateinamen.</span><span class="sxs-lookup"><span data-stu-id="69ce7-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="69ce7-p102">Kurs ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="69ce7-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="69ce7-p103">Verwenden Sie die Metadaten im oberen Bereich des diese Datei als Vorlage. Nichts ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="69ce7-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="69ce7-111">Navigieren Sie in der [Alchemy Partner-Portal](https://alchemyportal.azurewebsites.net)nach unten zum Abschnitt **Customer Erkenntnisse Title:** und verwenden, die als Ausgangspunkt zeigen für Ihr H1 Titel für den Einblick.</span><span class="sxs-lookup"><span data-stu-id="69ce7-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="69ce7-p104">Alchemy Insights müssen nur ein einzelnes H1 am Anfang oder in der Produktion getrennt wird. H2s nicht in diesem Fall verwenden **Fett** oder anderen Konventionen zur Kennzeichnung von getrennte Abschnitte zu rendern.</span><span class="sxs-lookup"><span data-stu-id="69ce7-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="69ce7-114">Im nächsten Schritt im Textkörper mit der Entwurf Material im Abschnitt Customer Einblicke in der Regel Alchemy Seite ausfüllen.</span><span class="sxs-lookup"><span data-stu-id="69ce7-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="69ce7-115">Listen mit Aufzählungszeichen sind in Ordnung</span><span class="sxs-lookup"><span data-stu-id="69ce7-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="69ce7-116">Nummerierte Listen zu</span><span class="sxs-lookup"><span data-stu-id="69ce7-116">Numbered lists too</span></span>
    1. <span data-ttu-id="69ce7-117">**Fett** und *kursiv formatiert* werden a-ok</span><span class="sxs-lookup"><span data-stu-id="69ce7-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="69ce7-118">Links werden entweder **"Links zu Web" / externe** OR **Deep-Links von Benutzeroberflächenelementen**, die nicht über interne Links.</span><span class="sxs-lookup"><span data-stu-id="69ce7-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="69ce7-p105">Und dies ist wirklich noch etwas zu lang. Bewährt hat ungefähr 400 Zeichen:</span><span class="sxs-lookup"><span data-stu-id="69ce7-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="69ce7-p106">Wenn Ihre Inhalte bereit ist, ziehen Sie es der live-Verzweigung. Wechseln Sie zu der [Alchemy Partner-Portal](https://alchemyportal.azurewebsites.net) , und geben Sie den Dateinamen in das Feld Url. Stellen Sie sicher, Erkenntnisse überprüft und veröffentlicht "Ja", sagt, und klicken Sie dann auf Regel aktualisieren. **(Dies sieht schönere in der neuen Version des Portals - bald freigeben.)** 
 ![-Url-Feld](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="69ce7-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

