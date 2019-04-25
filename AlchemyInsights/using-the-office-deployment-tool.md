---
title: Verwenden des Office-BereitstellungsTools
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: c7e0e96f225030590fdd516eaf3115c93a6335b6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423182"
---
# <a name="using-the-office-deployment-tool-odt"></a>Verwenden des Office-BereitstellungsTools (ODT)

Sie verwenden das Office-Bereitstellungs Tool (ODT) für die Bereitstellung von Office 365-Versionen von Office. Das Office-Bereitstellungs Tool (Setup. exe) wird von der Befehlszeile aus ausgeführt und verwendet eine Konfigurations-XML-Datei, um zu bestimmen, welche Einstellungen bei der Bereitstellung von Office gelten sollen.
  
1. Laden Sie die neueste Version des Office-BereitstellungsTools aus dem [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065)herunter.
    
2. Verwenden Sie das [Office-Anpassungs Tool (OAT)](https://config.office.com) , um Ihre Bereitstellungseinstellungen auszuwählen und die Konfigurations-XML-Datei zu erstellen. Exportieren Sie die Konfigurationsdatei, und platzieren Sie Sie lokal im gleichen Ordner, in dem sich Setup. exe befindet. 
    
    **Hinweis:** Probleme mit der Office-Installation entstehen häufig aufgrund falsch konfigurierter oder ungültige Konfigurationsdateien. Um solche Probleme zu vermeiden, sollten Sie das Office-Anpassungs Tool verwenden, um die Konfigurationsdatei zu erstellen. Sie können auch vorhandene Konfigurationsdateien in das Office-Anpassungs Tool importieren. 
    
3. Wechseln Sie an einer Eingabeaufforderungen mit erhöhten Rechten zu dem Speicherort, an dem sich Setup. exe befindet, und führen Sie das Office-Bereitstellungs Tool im Downloadmodus aus, und geben Sie die soeben gespeicherte Konfigurationsdatei an. In diesem Beispiel lautet die Konfigurationsdatei "Configuration. xml":
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Führen Sie das Office-Bereitstellungs Tool im configure-Modus aus, und geben Sie die Konfigurationsdatei an.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **Hinweis:** Sie müssen diesen Schritt auf dem Clientcomputer ausführen, auf dem Sie Office installieren möchten, und Sie müssen über lokale Administratorberechtigungen auf diesem Computer verfügen. 
    
Weitere Informationen zur Verwendung des Office-BereitstellungsTools für Office 365 proPlus-Bereitstellungsszenarien finden Sie unter [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Weitere Informationen zur Verwendung des Office-Anpassungstools finden Sie unter [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
  

