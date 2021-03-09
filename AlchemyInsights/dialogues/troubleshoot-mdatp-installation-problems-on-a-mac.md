---
title: Behandeln von Problemen bei der MDATP-Installation auf einem Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568623"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="5e74e-102">Behandeln von Problemen bei der MDATP-Installation auf einem Mac</span><span class="sxs-lookup"><span data-stu-id="5e74e-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="5e74e-103">Wenn bei der manuellen Installation ein Fehler auftritt, wird auf der Seite **Zusammenfassung** des Installations-Assistenten der folgende Fehler angezeigt:</span><span class="sxs-lookup"><span data-stu-id="5e74e-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="5e74e-104">"Bei der Installation ist ein Fehler aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="5e74e-104">"An error occurred during installation.</span></span> <span data-ttu-id="5e74e-105">Beim Installer ist ein Fehler aufgetreten, der zu einem Fehler bei der Installation führte.</span><span class="sxs-lookup"><span data-stu-id="5e74e-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="5e74e-106">Wenden Sie sich an den Softwarehersteller, um Unterstützung zu erhalten."</span><span class="sxs-lookup"><span data-stu-id="5e74e-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="5e74e-107">Bei MDM-Bereitstellungen zeigt die Seite auch einen allgemeinen Installationsfehler an.</span><span class="sxs-lookup"><span data-stu-id="5e74e-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="5e74e-108">Obwohl endbenutzern keine genauen Fehler angezeigt werden, wird eine Protokolldatei mit Dem Installationsfortschritt in **/Library/Logs/Microsoft/mdatp/install.log gespeichert.**</span><span class="sxs-lookup"><span data-stu-id="5e74e-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="5e74e-109">Jede Installationssitzung wird an diese Protokolldatei angefügt.</span><span class="sxs-lookup"><span data-stu-id="5e74e-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="5e74e-110">Verwenden Sie zum Ausgabe der letzten Installationssitzung `sed` .</span><span class="sxs-lookup"><span data-stu-id="5e74e-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="5e74e-111">Weitere Informationen finden Sie unter [Beheben von Installationsproblemen für Microsoft Defender ATP für Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span><span class="sxs-lookup"><span data-stu-id="5e74e-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
