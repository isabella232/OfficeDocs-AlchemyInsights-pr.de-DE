---
title: Verwenden des Office-Bereitstellungstools
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085831"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="1c93b-102">Verwenden des Office-Bereitstellungstools (ODT)</span><span class="sxs-lookup"><span data-stu-id="1c93b-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="1c93b-103">Verwenden Sie das Office-Bereitstellungs Tool (ODT), um Office 365 Versionen von Office bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="1c93b-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="1c93b-104">Das Office-Bereitstellungs Tool (setupodt.exe) wird über die Befehlszeile ausgeführt und verwendet eine Konfigurations-XML-Datei, um festzulegen, welche Einstellungen beim Bereitstellen von Office angewendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="1c93b-104">The Office Deployment Tool (setupodt.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="1c93b-105">Laden Sie die neueste Version des Office-Bereitstellungstools aus dem [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065)herunter.</span><span class="sxs-lookup"><span data-stu-id="1c93b-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="1c93b-106">Verwenden Sie das [Office-Anpassungs Tool (OAT)](https://config.office.com) , um Ihre Bereitstellungseinstellungen auszuwählen und die XML-Konfigurationsdatei zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="1c93b-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="1c93b-107">Exportieren Sie die Konfigurationsdatei, und platzieren Sie Sie lokal in demselben Ordner, in dem sich die setupodt.exe befindet.</span><span class="sxs-lookup"><span data-stu-id="1c93b-107">Export the configuration file and place it locally on the same folder where the setupodt.exe resides.</span></span>

    <span data-ttu-id="1c93b-108">**Hinweis:** Probleme mit der Office-Installation treten häufig aufgrund falsch konfigurierter oder ungültige Konfigurationsdateien auf.</span><span class="sxs-lookup"><span data-stu-id="1c93b-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="1c93b-109">Um solche Probleme zu vermeiden, sollten Sie das Office-Anpassungs Tool verwenden, um die Konfigurationsdatei zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="1c93b-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="1c93b-110">Sie können auch vorhandene Konfigurationsdateien in das Office-Anpassungs Tool importieren.</span><span class="sxs-lookup"><span data-stu-id="1c93b-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="1c93b-111">Wechseln Sie an einer Eingabeaufforderung mit erhöhten Rechten zu dem Speicherort, an dem sich setupodt.exe befindet, und führen Sie das Office-Bereitstellungs Tool im Downloadmodus aus, und geben Sie die soeben gespeicherte Konfigurationsdatei an.</span><span class="sxs-lookup"><span data-stu-id="1c93b-111">From an elevated command prompt, switch to the location where setupodt.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="1c93b-112">In diesem Beispiel wird die Konfigurationsdatei Configuration.xml benannt:</span><span class="sxs-lookup"><span data-stu-id="1c93b-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setupodt.exe /download Configuration.xml```

<span data-ttu-id="1c93b-113">4. führen Sie das Office-Bereitstellungs Tool im configure-Modus aus, und geben Sie die Konfigurationsdatei an.</span><span class="sxs-lookup"><span data-stu-id="1c93b-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setupodt.exe /configure Configuration.xml```

<span data-ttu-id="1c93b-114">**Hinweis:** Sie müssen diesen Schritt auf dem Clientcomputer ausführen, auf dem Sie Office installieren möchten, und Sie benötigen lokale Administratorberechtigungen auf diesem Computer.</span><span class="sxs-lookup"><span data-stu-id="1c93b-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="1c93b-115">Weitere Informationen zur Verwendung des Office-Bereitstellungstools für Ihre Microsoft 365-Apps für Enterprise-Bereitstellungsszenarien finden Sie unter [Übersicht über das Office-Bereitstellungstool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="1c93b-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="1c93b-116">Weitere Informationen zur Verwendung des Office-Anpassungstools finden Sie unter [Übersicht über das Office-Anpassungstool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="1c93b-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
