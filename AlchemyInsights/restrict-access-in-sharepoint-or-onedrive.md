---
title: Einschränken des Zugriffs in SharePoint oder OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715883"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Einschränken des Zugriffs in SharePoint oder OneDrive

In SharePoint und OneDrive schränken Sie den Zugriff auf Elemente wie Dateien, Ordner und Listen ein, indem Sie nur Gruppen oder Personen Zugriff gewähren, auf die Sie Zugriff haben möchten. Standardmäßig werden Berechtigungen in SharePoint von oben in der Hierarchie vererbt. Eine Datei erbt also Ihre Berechtigungen aus dem Ordner, der Ihre Berechtigungen von der Bibliothek erbt, die ihre Berechtigungen von der Website erbt.
  
Sie können auf einer höheren Ebene freigeben (beispielsweisedurch Freigabe einer ganzen Website) und dann die Vererbung aufbrechen, wenn Sie nicht alle Elemente auf der Website freigeben möchten. Dies wird jedoch nicht empfohlen, da die Verwaltung der Berechtigungen in Zukunft komplexer und verwirrender wird. Hier sehen Sie, was Sie stattdessen tun könnten:
  
- Wenn Sie beispielsweise alle Inhalte eines Ordners mit Ausnahme einer einzigen Datei freigeben möchten, müssen Sie die Datei an einen neuen Speicherort versetzen, der nicht freigegeben ist.
    
- Wenn Sie über zwei Unterordner in einem Ordner verfügen und einen Unterordner mit den Gruppen a und B freigeben und nur Gruppen Zugriff auf den zweiten Unterordner zulassen möchten, geben Sie den übergeordneten Ordner mit Gruppe a frei, und fügen Sie Gruppe b dem ersten Unterordner hinzu.
    
[Beenden der Freigabe einer Datei oder eines Ordners](https://go.microsoft.com/fwlink/?linkid=2008861)
  

