---
title: Probleme mit dem bedingten Zugriff
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013951"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="16d42-102">Probleme mit dem bedingten Zugriff</span><span class="sxs-lookup"><span data-stu-id="16d42-102">Conditional access issues</span></span>

<span data-ttu-id="16d42-103">**Beheben von Problemen mit der Anmeldediagnose**</span><span class="sxs-lookup"><span data-stu-id="16d42-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="16d42-104">Sie können schnell herausfinden, was passiert ist, oder Probleme im Zusammenhang mit der Benutzer anmeldung mithilfe der [Anmeldediagnose diagnostizieren:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="16d42-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="16d42-105">Starten Sie die Anmeldediagnose.</span><span class="sxs-lookup"><span data-stu-id="16d42-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="16d42-106">Suchen Sie das zu analysierende Ereignis, indem Sie die Details zu Benutzer, Anwendung, Zeitpunkt der Anmeldung, Anforderungs-ID oder Korrelations-ID eingeben.</span><span class="sxs-lookup"><span data-stu-id="16d42-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="16d42-107">Überprüfen Sie die Diagnoseergebnisse, in denen die Details zu den Vorfall und die Aktionen angezeigt werden, die Sie ergreifen können, um Änderungen vorzunehmen (falls Änderungen erforderlich sind).</span><span class="sxs-lookup"><span data-stu-id="16d42-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="16d42-108">**Schritte zur Problembehandlung bei einer Anmeldung**</span><span class="sxs-lookup"><span data-stu-id="16d42-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="16d42-109">Navigieren Sie zur Azure AD-Anmeldeseite.</span><span class="sxs-lookup"><span data-stu-id="16d42-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="16d42-110">Filtern Sie Anmeldungen nach Benutzer, Zeitraum, Anwendung, Status, Client-App und so weiter.</span><span class="sxs-lookup"><span data-stu-id="16d42-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="16d42-111">Wählen Sie ein Anmeldeereignis aus, und zeigen Sie die Registerkarte "Bedingter Zugriff" an, um zu sehen, welche Richtlinien ausgewertet wurden.</span><span class="sxs-lookup"><span data-stu-id="16d42-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="16d42-112">Klicken Sie auf die Zeile einer Richtlinie, um die Richtliniendetails anzuzeigen und zu verstehen, warum sie angewendet wurde.</span><span class="sxs-lookup"><span data-stu-id="16d42-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="16d42-113">**Tools zur Problembehandlung für eine Richtlinie für bedingten Zugriff**</span><span class="sxs-lookup"><span data-stu-id="16d42-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="16d42-114">Im Nur-Berichts-Modus können Sie eine Richtlinie auswerten, ohne sich auf die Benutzer auszu auswirken.</span><span class="sxs-lookup"><span data-stu-id="16d42-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="16d42-115">Mit dem Tool "Was-wäre-wenn" können Sie Anmeldeereignisse simulieren und sehen, welche Richtlinien gelten.</span><span class="sxs-lookup"><span data-stu-id="16d42-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="16d42-116">Die Arbeitsmappe "Einblicke und Berichterstellung" zeigt die Auswirkungen jeder Richtlinie in Echtzeit an.</span><span class="sxs-lookup"><span data-stu-id="16d42-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="16d42-117">**Grundlegende Schutzrichtlinien**</span><span class="sxs-lookup"><span data-stu-id="16d42-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="16d42-118">Baseline Protection policies have been deprecated.</span><span class="sxs-lookup"><span data-stu-id="16d42-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="16d42-119">Sie werden nicht mehr erzwungen und werden bald aus dem Azure-Portal entfernt.</span><span class="sxs-lookup"><span data-stu-id="16d42-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="16d42-120">Es wird empfohlen, [Die Sicherheitseinstellungen zu aktivieren.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)</span><span class="sxs-lookup"><span data-stu-id="16d42-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="16d42-121">Weitere Informationen zum bedingten Zugriff finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="16d42-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="16d42-122">[Bewährte Methoden für bedingten Zugriff in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Bedingungen im bedingten Zugriff](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Steuerelemente im bedingten Zugriff](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Speicherorte im bedingten Zugriff](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="16d42-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
