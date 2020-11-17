---
title: Fragen zur Verwendung des Office-Bereitstellungstools (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086155"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Fragen zur Verwendung des Office-Bereitstellungstools (ODT)

Laden Sie das Office-Bereitstellungstool aus dem [Microsoft Download Center herunter](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Führen Sie nach dem Herunterladen der Datei die selbstextrahierende ausführbare Datei aus, die die ausführbare Datei des Office-Bereitstellungstools (setupodt.exe) und eine Beispielkonfigurationsdatei (configuration.xml) enthält.
  
 **So schließen Sie Microsoft 365-Apps für Enterprise-Produkte von Clientcomputern aus oder entfernen Sie:**
  
Bei der Installation von Microsoft 365-Apps für Enterprise können Sie bestimmte Produkte ausschließen. Führen Sie dazu die Schritte für die Installation von Office mit dem ODT aus, fügen Sie jedoch das ExcludeApp-Element in der Konfigurationsdatei hinzu. In dieser Konfigurationsdatei werden beispielsweise alle Microsoft 365-Apps für Enterprise-Produkte mit Ausnahme von Publisher installiert:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Übersicht über das Office-Bereitstellungstool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

