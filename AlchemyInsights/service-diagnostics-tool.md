---
title: Dienstdiagnosetool für Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590302"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="8a9db-102">Dienstdiagnosetool für Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="8a9db-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="8a9db-103">Windows Virtual Desktop (WVD) bietet ein Diagnosetool, mit dem Administratoren Fehler über eine einzelne Schnittstelle erkennen können.</span><span class="sxs-lookup"><span data-stu-id="8a9db-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="8a9db-104">Dieses Tool protokolliert diagnosebezogene Informationen immer dann, wenn WVD von einer Person verwendet wird, der eine WVD-Rolle zugewiesen wurde.</span><span class="sxs-lookup"><span data-stu-id="8a9db-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="8a9db-105">Jedes Protokoll enthält Informationen zur WVD-Rolle, die an der Aktivität beteiligt ist, die Fehlermeldungen, die während der Sitzung angezeigt werden, und die Informationen zum Mandanten und Benutzer.</span><span class="sxs-lookup"><span data-stu-id="8a9db-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="8a9db-106">Mit den folgenden Schritten kann Azure Log Analytics so konfiguriert werden, dass das vom Diagnosetool erstellte Aktivitätsprotokoll erfasst wird:</span><span class="sxs-lookup"><span data-stu-id="8a9db-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="8a9db-107">Erstellen eines Protokollanalysearbeitsbereichs mit dem [Azure-Portal](https://go.microsoft.com/fwlink/?linkid=2129500) oder über [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="8a9db-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="8a9db-108">[Verbinden von Windows-Computern mit Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="8a9db-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="8a9db-109">Sie erhalten die Arbeitsbereichs-ID und den Primärschlüssel Ihres Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="8a9db-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="8a9db-110">Der Setup-Assistent benötigt diese Informationen, um den Agent ordnungsgemäß zu konfigurieren und um sicherzustellen, dass er mit Azure Monitor kommunizieren kann.</span><span class="sxs-lookup"><span data-stu-id="8a9db-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="8a9db-111">[Diagnosedaten in den Arbeitsbereich übertragen](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="8a9db-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="8a9db-112">Sie können Diagnosedaten aus dem WVD-Mandanten in Log Analytics für Ihren Arbeitsbereich übertragen.</span><span class="sxs-lookup"><span data-stu-id="8a9db-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="8a9db-113">[Identifizieren und Diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) von Problemen, die in Bezug auf WVD intern oder extern sind.</span><span class="sxs-lookup"><span data-stu-id="8a9db-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="8a9db-114">Weitere Informationen zum Konfigurieren des Dienstdiagnosetools für WVD finden Sie unter „Verwenden von Log Analytics für die Diagnosefunktion“.</span><span class="sxs-lookup"><span data-stu-id="8a9db-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>