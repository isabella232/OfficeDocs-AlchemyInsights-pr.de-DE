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
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="f4270-102">Verwenden des Office-BereitstellungsTools (ODT)</span><span class="sxs-lookup"><span data-stu-id="f4270-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="f4270-103">Sie verwenden das Office-Bereitstellungs Tool (ODT) für die Bereitstellung von Office 365-Versionen von Office.</span><span class="sxs-lookup"><span data-stu-id="f4270-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="f4270-104">Das Office-Bereitstellungs Tool (Setup. exe) wird von der Befehlszeile aus ausgeführt und verwendet eine Konfigurations-XML-Datei, um zu bestimmen, welche Einstellungen bei der Bereitstellung von Office gelten sollen.</span><span class="sxs-lookup"><span data-stu-id="f4270-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="f4270-105">Laden Sie die neueste Version des Office-BereitstellungsTools aus dem [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065)herunter.</span><span class="sxs-lookup"><span data-stu-id="f4270-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="f4270-106">Verwenden Sie das [Office-Anpassungs Tool (OAT)](https://config.office.com) , um Ihre Bereitstellungseinstellungen auszuwählen und die Konfigurations-XML-Datei zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="f4270-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="f4270-107">Exportieren Sie die Konfigurationsdatei, und platzieren Sie Sie lokal im gleichen Ordner, in dem sich Setup. exe befindet.</span><span class="sxs-lookup"><span data-stu-id="f4270-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="f4270-108">**Hinweis:** Probleme mit der Office-Installation entstehen häufig aufgrund falsch konfigurierter oder ungültige Konfigurationsdateien.</span><span class="sxs-lookup"><span data-stu-id="f4270-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="f4270-109">Um solche Probleme zu vermeiden, sollten Sie das Office-Anpassungs Tool verwenden, um die Konfigurationsdatei zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="f4270-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="f4270-110">Sie können auch vorhandene Konfigurationsdateien in das Office-Anpassungs Tool importieren.</span><span class="sxs-lookup"><span data-stu-id="f4270-110">You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="f4270-111">Wechseln Sie an einer Eingabeaufforderungen mit erhöhten Rechten zu dem Speicherort, an dem sich Setup. exe befindet, und führen Sie das Office-Bereitstellungs Tool im Downloadmodus aus, und geben Sie die soeben gespeicherte Konfigurationsdatei an.</span><span class="sxs-lookup"><span data-stu-id="f4270-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="f4270-112">In diesem Beispiel lautet die Konfigurationsdatei "Configuration. xml":</span><span class="sxs-lookup"><span data-stu-id="f4270-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="f4270-113">Führen Sie das Office-Bereitstellungs Tool im configure-Modus aus, und geben Sie die Konfigurationsdatei an.</span><span class="sxs-lookup"><span data-stu-id="f4270-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="f4270-114">**Hinweis:** Sie müssen diesen Schritt auf dem Clientcomputer ausführen, auf dem Sie Office installieren möchten, und Sie müssen über lokale Administratorberechtigungen auf diesem Computer verfügen.</span><span class="sxs-lookup"><span data-stu-id="f4270-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="f4270-115">Weitere Informationen zur Verwendung des Office-BereitstellungsTools für Office 365 proPlus-Bereitstellungsszenarien finden Sie unter [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="f4270-115">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="f4270-116">Weitere Informationen zur Verwendung des Office-Anpassungstools finden Sie unter [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="f4270-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

