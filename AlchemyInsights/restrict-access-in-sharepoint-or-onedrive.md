---
title: Einschränken des Zugriffs in SharePoint oder OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551450"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Einschränken des Zugriffs in SharePoint oder OneDrive

In SharePoint und OneDrive schränken Sie den Zugriff auf Elemente wie Dateien, Ordner und Listen ein, indem Sie nur Gruppen oder Personen Zugriff gewähren, auf die Sie Zugriff haben möchten. Standardmäßig werden Berechtigungen in SharePoint von oben in der Hierarchie vererbt. Eine Datei erbt also Ihre Berechtigungen aus dem Ordner, der Ihre Berechtigungen von der Bibliothek erbt, die ihre Berechtigungen von der Website erbt.
  
Sie können auf einer höheren Ebene freigeben (beispielsweisedurch Freigabe einer ganzen Website) und dann die Vererbung aufbrechen, wenn Sie nicht alle Elemente auf der Website freigeben möchten. Dies wird jedoch nicht empfohlen, da die Verwaltung der Berechtigungen in Zukunft komplexer und verwirrender wird. Hier sehen Sie, was Sie stattdessen tun könnten:
  
- Wenn Sie beispielsweise alle Inhalte eines Ordners mit Ausnahme einer einzigen Datei freigeben möchten, müssen Sie die Datei an einen neuen Speicherort versetzen, der nicht freigegeben ist.
    
- Wenn Sie über zwei Unterordner in einem Ordner verfügen und einen Unterordner mit den Gruppen a und B freigeben und nur Gruppen Zugriff auf den zweiten Unterordner zulassen möchten, geben Sie den übergeordneten Ordner mit Gruppe a frei, und fügen Sie Gruppe b dem ersten Unterordner hinzu.
    
[Beenden der Freigabe einer Datei oder eines Ordners](https://go.microsoft.com/fwlink/?linkid=2008861)
  

