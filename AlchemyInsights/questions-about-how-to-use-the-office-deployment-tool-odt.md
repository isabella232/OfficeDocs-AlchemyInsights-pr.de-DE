---
title: Fragen zur Verwendung des Office-Bereitstellungstools (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36553539"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Fragen zur Verwendung des Office-Bereitstellungstools (ODT)

Laden Sie das Office-Bereitstellungstool aus dem [Microsoft Download Center herunter](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Führen Sie nach dem Download die selbst entpackende ausführbare Datei aus, die die ausführbare Datei (setup.exe) und eine Beispielkonfigurationsdatei (configuration.xml) für das Office-Bereitstellungstool enthält.
  
 **So schließen Sie Office 365 ProPlus-Produkte von Clientcomputern aus oder entfernen Sie:**
  
Bei der Installation von Office 365 ProPlus können Sie bestimmte Produkte ausschließen. Führen Sie dazu die Schritte für die Installation von Office mit dem Office-Bereitstellungstool aus, fügen Sie jedoch der Konfigurationsdatei das "ExcludeApp"-Element hinzu. Mit dieser Konfigurationsdatei werden z.B. alle Office 365 ProPlus-Produkte mit Ausnahme von Publisher installiert:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Übersicht über das Office-Bereitstellungstool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

