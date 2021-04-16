---
title: Fragen zur Verwendung des Office-Bereitstellungstools (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 20e0b6aa3c298ee0a4291c3da6ae46978177e81f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790331"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="5aa25-102">Fragen zur Verwendung des Office-Bereitstellungstools (ODT)</span><span class="sxs-lookup"><span data-stu-id="5aa25-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="5aa25-103">Laden Sie das Office-Bereitstellungstool aus dem [Microsoft Download Center herunter](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="5aa25-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="5aa25-104">Führen Sie nach dem Download die selbst entpackende ausführbare Datei aus, die die ausführbare Datei (setup.exe) und eine Beispielkonfigurationsdatei (configuration.xml) für das Office-Bereitstellungstool enthält.</span><span class="sxs-lookup"><span data-stu-id="5aa25-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="5aa25-105">**So schließen Sie Microsoft 365 Apps for Enterprise-Produkte von Clientcomputern aus, oder entfernen Sie diese:**</span><span class="sxs-lookup"><span data-stu-id="5aa25-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="5aa25-106">Bei der Installation von Microsoft 365 Apps for Enterprise können Sie bestimmte Produkte ausschließen.</span><span class="sxs-lookup"><span data-stu-id="5aa25-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="5aa25-107">Führen Sie dazu die Schritte für die Installation von Office mit dem ODT aus, fügen Sie jedoch das ExcludeApp-Element in der Konfigurationsdatei hinzu.</span><span class="sxs-lookup"><span data-stu-id="5aa25-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="5aa25-108">Mit dieser Konfigurationsdatei werden beispielsweise alle Microsoft 365 Apps for Enterprise-Produkte mit Ausnahme von Publisher installiert:</span><span class="sxs-lookup"><span data-stu-id="5aa25-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="5aa25-109">Übersicht über das Office-Bereitstellungstool</span><span class="sxs-lookup"><span data-stu-id="5aa25-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

