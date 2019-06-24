---
title: Fix 0x8004de40-Fehler in OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133976"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="31c9e-102">Fix 0x8004de40-Fehler in OneDrive</span><span class="sxs-lookup"><span data-stu-id="31c9e-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="31c9e-103">Wenn Sie einen 0x8004de40-Fehler mit OneDrive erhalten:</span><span class="sxs-lookup"><span data-stu-id="31c9e-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="31c9e-104">Starten Sie den betroffenen Computer neu, während eine Verbindung mit ihrer Acitve-Verzeichnisdomäne besteht.</span><span class="sxs-lookup"><span data-stu-id="31c9e-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="31c9e-105">Wenn das Problem durch einen Neustart nicht behoben werden kann, trennen Sie die Verbindung und fügen Sie Ihr Gerät von Azure AD wieder hinzu.</span><span class="sxs-lookup"><span data-stu-id="31c9e-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="31c9e-106">**Hinweis**: Wenn Sie diese Schritte ausführen, sollten Sie sich im Unternehmensnetzwerk befinden.</span><span class="sxs-lookup"><span data-stu-id="31c9e-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="31c9e-107">Führen Sie diese Schritte nicht aus, wenn Sie nicht in der Lage sind, eine Verbindung mit Ihrer Unternehmensinfrastruktur herzustellen (beispielsweise auf Reisen).</span><span class="sxs-lookup"><span data-stu-id="31c9e-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="31c9e-108">Öffnen Sie die Eingabeaufforderung mit erhöhten Rechten.</span><span class="sxs-lookup"><span data-stu-id="31c9e-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="31c9e-109">Klicken Sie zum Öffnen einer Eingabeaufforderung mit erhöhten Rechten auf- **Start**, klicken Sie mit der rechten Maustaste auf **Eingabeaufforderung**, und klicken Sie dann auf **als Administrator ausführen**.</span><span class="sxs-lookup"><span data-stu-id="31c9e-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="31c9e-110">Geben Sie *dsregcmd/Leave* ein, und drücken **Sie die Eingabe**Taste.</span><span class="sxs-lookup"><span data-stu-id="31c9e-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="31c9e-111">Geben Sie nach Abschluss *dsregcmd/Join* ein, und drücken **Sie die Eingabe**Taste.</span><span class="sxs-lookup"><span data-stu-id="31c9e-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="31c9e-112">Schließen Sie nach Abschluss der Eingabeaufforderung.</span><span class="sxs-lookup"><span data-stu-id="31c9e-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="31c9e-113">Starten Sie den Computer neu, und melden Sie sich bei OneDrive an.</span><span class="sxs-lookup"><span data-stu-id="31c9e-113">Reboot the computer, and log into OneDrive.</span></span>