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
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="29006-102">Using the Office Deployment Tool (ODT)</span><span class="sxs-lookup"><span data-stu-id="29006-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="29006-p101">Verwenden Sie Office Deployment Tool (ODT), um Office 365-Versionen von Office bereitzustellen. Office-Bereitstellungstool (setup.exe) über die Befehlszeile ausgeführt wird und eine XML-Konfigurationsdatei um zu bestimmen, welche Einstellungen Sie übernehmen bei der Bereitstellung von Office verwendet.</span><span class="sxs-lookup"><span data-stu-id="29006-p101">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office. The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="29006-105">Laden Sie die neueste Version von Office-Bereitstellungstool aus dem [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065)herunter.</span><span class="sxs-lookup"><span data-stu-id="29006-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="29006-p102">Verwenden Sie das [Office-Anpassungstool (OAT)](https://config.office.com) , wählen Sie Ihre Bereitstellung Voreinstellungen und Erstellen der XML-Konfigurationsdatei. Exportieren Sie die Konfigurationsdatei, und legen Sie es lokal auf demselben Ordner, in dem die setup.exe befindet.</span><span class="sxs-lookup"><span data-stu-id="29006-p102">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="29006-p103">**Hinweis:** Office-Installation Probleme häufig Fälligkeitsdatum, falsch konfigurierter auftreten oder Konfigurationsdateien falsch formatiert. Um solche Probleme zu vermeiden, sollten Sie Office-Anpassungstool verwenden, um die Konfigurationsdatei zu erstellen. Sie können auch vorhandene Konfigurationsdateien in Office-Anpassungstool importieren.</span><span class="sxs-lookup"><span data-stu-id="29006-p103">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files. To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file. You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="29006-p104">Aus einer Eingabeaufforderung mit erhöhten Rechten wechseln Sie zum Speicherort setup.exe und führen Sie das Office-Bereitstellungstool im Modus downloadmodusaus, und geben Sie die Konfigurationsdatei, die Sie gerade gespeichert. In diesem Beispiel wird die Konfigurationsdatei mit der Bezeichnung "Configuration.xml":</span><span class="sxs-lookup"><span data-stu-id="29006-p104">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved. In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="29006-113">Führen Sie das Office-Bereitstellungstool im Modus Konfiguration aus, und geben Sie die Konfigurationsdatei.</span><span class="sxs-lookup"><span data-stu-id="29006-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="29006-114">**Hinweis:** Dieser Schritt muss auf dem Clientcomputer ausgeführt werden, auf dem Sie Office installieren möchten, und Sie benötigen lokale Administratorberechtigungen auf diesem Computer.</span><span class="sxs-lookup"><span data-stu-id="29006-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="29006-p105">Weitere Informationen zur Verwendung von Office-Bereitstellungstools für Office 365 ProPlus Bereitstellungsszenarien finden Sie unter [Übersicht über die Office-Bereitstellungstools](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Weitere Informationen zum Verwenden des Office-Anpassungstools finden Sie unter [Übersicht über Office-Anpassungstool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="29006-p105">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

