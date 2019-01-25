---
title: Mithilfe des Office-Bereitstellungstools
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29469791"
---
# <a name="using-the-office-deployment-tool-odt"></a>Using the Office Deployment Tool (ODT)

Verwenden Sie Office Deployment Tool (ODT), um Office 365-Versionen von Office bereitzustellen. Office-Bereitstellungstool (setup.exe) über die Befehlszeile ausgeführt wird und eine XML-Konfigurationsdatei um zu bestimmen, welche Einstellungen Sie übernehmen bei der Bereitstellung von Office verwendet.
  
1. Laden Sie die neueste Version von Office-Bereitstellungstool aus dem [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065)herunter.
    
2. Verwenden Sie das [Office-Anpassungstool (OAT)](https://config.office.com) , wählen Sie Ihre Bereitstellung Voreinstellungen und Erstellen der XML-Konfigurationsdatei. Exportieren Sie die Konfigurationsdatei, und legen Sie es lokal auf demselben Ordner, in dem die setup.exe befindet. 
    
    **Hinweis:** Office-Installation Probleme häufig Fälligkeitsdatum, falsch konfigurierter auftreten oder Konfigurationsdateien falsch formatiert. Um solche Probleme zu vermeiden, sollten Sie Office-Anpassungstool verwenden, um die Konfigurationsdatei zu erstellen. Sie können auch vorhandene Konfigurationsdateien in Office-Anpassungstool importieren. 
    
3. Aus einer Eingabeaufforderung mit erhöhten Rechten wechseln Sie zum Speicherort setup.exe und führen Sie das Office-Bereitstellungstool im Modus downloadmodusaus, und geben Sie die Konfigurationsdatei, die Sie gerade gespeichert. In diesem Beispiel wird die Konfigurationsdatei mit der Bezeichnung "Configuration.xml":
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Führen Sie das Office-Bereitstellungstool im Modus Konfiguration aus, und geben Sie die Konfigurationsdatei.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Hinweis:** Dieser Schritt muss auf dem Clientcomputer ausgeführt werden, auf dem Sie Office installieren möchten, und Sie benötigen lokale Administratorberechtigungen auf diesem Computer. 
    
Weitere Informationen zur Verwendung von Office-Bereitstellungstools für Office 365 ProPlus Bereitstellungsszenarien finden Sie unter [Übersicht über die Office-Bereitstellungstools](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Weitere Informationen zum Verwenden des Office-Anpassungstools finden Sie unter [Übersicht über Office-Anpassungstool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
  

