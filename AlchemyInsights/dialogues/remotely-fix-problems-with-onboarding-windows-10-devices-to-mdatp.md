---
title: Remotebehebt Probleme beim Onboarding von Windows 10-Geräten in Microsoft Defender Advanced Threat Protection
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
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50530006"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="30d3e-102">Remotebehebt Probleme beim Onboarding von Windows 10-Geräten in Microsoft Defender Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="30d3e-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="30d3e-103">Wenn Sie auf den Remotecomputer zugreifen können, führen Sie die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="30d3e-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="30d3e-104">Laden Sie das [Clientverbindungsuntersuchung](https://go.microsoft.com/fwlink/?linkid=2143466)-Diagnosetool herunter.</span><span class="sxs-lookup"><span data-stu-id="30d3e-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="30d3e-105">Extrahieren Sie MDATPAnalyzer.cmd, und führen Sie es aus.</span><span class="sxs-lookup"><span data-stu-id="30d3e-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="30d3e-106">Suchen Sie das Diagnoseprotokoll im Ordner MDATPClientAnalyzerResult, der sich im selben Ordner befindet, in dem das Tool Analyzer heruntergeladen wurde.</span><span class="sxs-lookup"><span data-stu-id="30d3e-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="30d3e-107">Um Probleme mit Konnektivitäts- oder Internetproxyeinstellungen zu finden, überprüfen Sie die Protokolldatei MDATPClientAnalyzer.txt.</span><span class="sxs-lookup"><span data-stu-id="30d3e-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="30d3e-108">Weitere Informationen finden Sie unter [Probleme mit Onboardingcomputern](https://go.microsoft.com/fwlink/?linkid=2143634).</span><span class="sxs-lookup"><span data-stu-id="30d3e-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
