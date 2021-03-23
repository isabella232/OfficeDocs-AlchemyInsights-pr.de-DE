---
title: Probleme beim Onboarding von Computern in Microsoft Defender für Endpunkt
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901566"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="fd35d-102">Probleme beim Onboarding von Computern in Microsoft Defender für Endpunkt</span><span class="sxs-lookup"><span data-stu-id="fd35d-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="fd35d-103">Möglicherweise haben Sie Probleme beim Onboarding von Computern in den MDE-Dienst.</span><span class="sxs-lookup"><span data-stu-id="fd35d-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="fd35d-104">Wenn Sie auf den Endbenutzercomputer zugreifen können, führen Sie die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="fd35d-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="fd35d-105">Laden Sie die neueste Vorschauversion des Diagnosetools zur [MDE-Clientanalyse](https://aka.ms/betamdeanalyzer) herunter.</span><span class="sxs-lookup"><span data-stu-id="fd35d-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="fd35d-106">Klicken Sie mit der rechten Maustaste auf **MDEClientAnalyzer.cmd** und wählen Sie „Als Administrator ausführen“ aus.</span><span class="sxs-lookup"><span data-stu-id="fd35d-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="fd35d-107">Befolgen Sie alle Hilfestellungen, die Ihnen in **MDEClientAnalyzer.htm** vorgeschlagen werden.</span><span class="sxs-lookup"><span data-stu-id="fd35d-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="fd35d-108">Weitere ausführliche Protokolle finden Sie im erstellten Unterordner namens **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="fd35d-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="fd35d-109">Wenn zusätzliche Anleitung nötig ist, wenden Sie sich an den [Support für Microsoft Defender für Endpunkt](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) und stellen Sie die resultierende Datei „MDEClientAnalyzerResult.zip“ zur Analyse zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="fd35d-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
