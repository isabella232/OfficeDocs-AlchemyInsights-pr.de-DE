---
title: Dienst Diagnosetool für Windows Virtual Desktop
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/14/2020
ms.locfileid: "49665824"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="c3c0c-102">Dienst Diagnosetool für Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="c3c0c-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="c3c0c-103">Windows Virtual Desktop (Oktober) bietet ein Diagnosetool, mit dem Administratoren Fehler über eine einzelne Schnittstelle identifizieren können.</span><span class="sxs-lookup"><span data-stu-id="c3c0c-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="c3c0c-104">Dieses Tool protokolliert Diagnose bezogene Informationen, wenn Oktober von einem Benutzer verwendet wird, dem eine Oktober-Rolle zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="c3c0c-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="c3c0c-105">Jedes Protokoll enthält Informationen über die an der Aktivität beteiligte Oktober-Rolle, die Fehlermeldungen, die während der Sitzung angezeigt werden, sowie Informationen über den Mandanten und den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="c3c0c-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="c3c0c-106">Azure Log Analytics kann so konfiguriert werden, dass das vom Diagnosetool erstellte Aktivitätsprotokoll erfasst wird.</span><span class="sxs-lookup"><span data-stu-id="c3c0c-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="c3c0c-107">Dazu gehen Sie so vor:</span><span class="sxs-lookup"><span data-stu-id="c3c0c-107">Here's how:</span></span>

1. <span data-ttu-id="c3c0c-108">Erstellen Sie einen Log Analytics-Arbeitsbereich mit dem [Azure-Portal](https://go.microsoft.com/fwlink/?linkid=2129500) oder [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="c3c0c-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="c3c0c-109">[Verbinden Sie Windows-Computer mit Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="c3c0c-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="c3c0c-110">Rufen Sie die Arbeitsbereichs-ID und den Primärschlüssel Ihres Arbeitsbereichs ab.</span><span class="sxs-lookup"><span data-stu-id="c3c0c-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="c3c0c-111">Der Setup-Assistent benötigt diese Informationen, um den Agent ordnungsgemäß zu konfigurieren und sicherzustellen, dass er mit Azure Monitor kommunizieren kann.</span><span class="sxs-lookup"><span data-stu-id="c3c0c-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="c3c0c-112">[Drücken Sie Diagnosedaten in den Arbeitsbereich](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="c3c0c-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="c3c0c-113">Sie können Diagnosedaten von Ihrem Oktober-Mandanten in die Protokollanalyse für Ihren Arbeitsbereich verschieben.</span><span class="sxs-lookup"><span data-stu-id="c3c0c-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="c3c0c-114">[Identifizieren und diagnostizieren](https://go.microsoft.com/fwlink/?linkid=2128338) Sie interne oder externe Probleme im Zusammenhang mit Oktober.</span><span class="sxs-lookup"><span data-stu-id="c3c0c-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="c3c0c-115">Weitere Informationen zum Konfigurieren des Dienst Diagnosetools für Oktober finden Sie unter [use Log Analytics for the Diagnostics Feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="c3c0c-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
