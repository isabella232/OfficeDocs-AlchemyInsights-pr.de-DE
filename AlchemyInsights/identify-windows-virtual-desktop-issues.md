---
title: Identifizieren von Problemen mit Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590295"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="71d89-102">Identifizieren von Problemen mit Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="71d89-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="71d89-103">Windows Virtual Desktop-Diagnose verwendet nur ein PowerShell-Cmdlet, enthält aber viele optionale Parameter, um Probleme einzugrenzen und zu isolieren.</span><span class="sxs-lookup"><span data-stu-id="71d89-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="71d89-104">Erste Schritte:</span><span class="sxs-lookup"><span data-stu-id="71d89-104">To get started:</span></span> 

1. <span data-ttu-id="71d89-105">Laden Sie das Windows Virtual Desktop PowerShell-Modul herunter, und importieren Sie es.</span><span class="sxs-lookup"><span data-stu-id="71d89-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="71d89-106">Weitere Informationen finden Sie unter [Windows Virtual Desktop-Cmdlets für Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span><span class="sxs-lookup"><span data-stu-id="71d89-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="71d89-107">Führen Sie das folgende Cmdlet aus, um sich bei Ihrem Konto anmelden:</span><span class="sxs-lookup"><span data-stu-id="71d89-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="71d89-108">Beispiel: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="71d89-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="71d89-109">**HINWEIS:** Alle Abfragen mit PowerShell müssen entweder die Parameter "-UserName" oder "-ActivityID" enthalten.</span><span class="sxs-lookup"><span data-stu-id="71d89-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="71d89-110">Informationen zu den Überwachungsfunktionen finden Sie unter [Protokollanalyse für die Diagnosefunktion](https://go.microsoft.com/fwlink/?linkid=2126847).</span><span class="sxs-lookup"><span data-stu-id="71d89-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="71d89-111">Führen Sie das folgende Cmdlet aus, um Diagnoseaktivitäten nach Benutzer zu filtern:</span><span class="sxs-lookup"><span data-stu-id="71d89-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="71d89-112">Beispiel: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="71d89-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="71d89-113">Es gibt eine Liste von Filtern, die Sie ausführen können, um Probleme zu diagnostizieren.</span><span class="sxs-lookup"><span data-stu-id="71d89-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="71d89-114">Weitere Informationen zur Diagnose von Problemen finden Sie unter [Ermitteln und Diagnostizieren von Problemen mit Windows Virtual Desktop](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="71d89-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="71d89-115">Weitere Informationen zu üblichen Fehlern finden Sie unter [Häufig auftretende Fehlerszenarien](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span><span class="sxs-lookup"><span data-stu-id="71d89-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
