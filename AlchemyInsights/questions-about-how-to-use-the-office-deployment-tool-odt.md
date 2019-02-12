---
title: Fragen zur Verwendung von Office Deployment Tool (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e91d40f872dd401ee210ac05eb39d64b6fb88027
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29925343"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="bc1c1-102">Fragen zur Verwendung von Office Deployment Tool (ODT)</span><span class="sxs-lookup"><span data-stu-id="bc1c1-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="bc1c1-103">Laden Sie das Office-Bereitstellungstool aus dem [Microsoft Download Center herunter](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="bc1c1-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="bc1c1-104">Führen Sie nach dem Download die selbst entpackende ausführbare Datei aus, die die ausführbare Datei (setup.exe) und eine Beispielkonfigurationsdatei (configuration.xml) für das Office-Bereitstellungstool enthält.</span><span class="sxs-lookup"><span data-stu-id="bc1c1-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="bc1c1-105">**Zum Ausschließen oder Entfernen von Office 365 ProPlus-Produkte von Client-Computern:**</span><span class="sxs-lookup"><span data-stu-id="bc1c1-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="bc1c1-p101">Wenn Sie Office 365 ProPlus installieren, können Sie bestimmte Produkte ausschließen. Führen Sie dazu die Schritte für die Installation von Office mit dem ODT aus, fügen Sie jedoch das ExcludeApp-Element in der Konfigurationsdatei hinzu. Mit dieser Konfigurationsdatei werden z. B. alle Office 365 ProPlus-Produkte mit Ausnahme von Publisher installiert:</span><span class="sxs-lookup"><span data-stu-id="bc1c1-p101">When installing Office 365 ProPlus, you can exclude specific products. To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file. For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="bc1c1-109">Übersicht über das Office-Bereitstellungstool</span><span class="sxs-lookup"><span data-stu-id="bc1c1-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

