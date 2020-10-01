---
title: Konfigurieren von Endpunkt-DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: d0363d6bdecdb266a5f4a3a14bd496ede6bb9931
ms.sourcegitcommit: 76b147af688f0dc39878a913a050c0e56af054a8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/29/2020
ms.locfileid: "48305442"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="f6cb0-102">Konfigurieren von Endpunkt-DLP</span><span class="sxs-lookup"><span data-stu-id="f6cb0-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="f6cb0-103">Microsoft Endpunkt-DLP bietet Ihnen die Möglichkeit, Schutz- und Überwachungsfunktionen von DLP auf vertrauliche Informationen auf Windows 10-Geräten zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="f6cb0-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="f6cb0-104">Nachdem die Geräte in die Geräteverwaltung integriert wurden, können Sie DLP-Richtlinien erstellen, um Schutzmaßnahmen für Objekte durchzusetzen.</span><span class="sxs-lookup"><span data-stu-id="f6cb0-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="f6cb0-105">Der Aktivitäten-Explorer kann verwendet werden, um die Aktivität für vertrauliche Elemente zu überwachen.</span><span class="sxs-lookup"><span data-stu-id="f6cb0-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="f6cb0-106">Weitere Informationen finden Sie unter [Onboarding von Geräten für die Geräteverwaltung](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="f6cb0-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="f6cb0-107">So führen Sie die ersten Schritte mit Endpunkt-DLP aus</span><span class="sxs-lookup"><span data-stu-id="f6cb0-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="f6cb0-108">Stellen Sie sicher, dass Sie über die geeignete SKU/Abonnementlizenzierung verfügen.</span><span class="sxs-lookup"><span data-stu-id="f6cb0-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="f6cb0-109">Weitere Informationen finden Sie unter [SKU/Abonnement-Lizenzierung](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="f6cb0-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="f6cb0-110">Überprüfen Sie die Berechtigungen, die erforderlich sind, um die Geräteverwaltung zu aktivieren, auf die Onboardingseite zuzugreifen oder die Geräteüberwachung ein- und auszuschalten.</span><span class="sxs-lookup"><span data-stu-id="f6cb0-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="f6cb0-111">Weitere Informationen finden Sie unter [Berechtigungen](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="f6cb0-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="f6cb0-112">Führen Sie ein Onboarding der Geräte in die Geräteverwaltung aus, indem Sie dem Verfahren für das Onboarding von Geräten folgen.</span><span class="sxs-lookup"><span data-stu-id="f6cb0-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="f6cb0-113">Wenn Sie die Option "Geräte-Onboarding (Vorschau)" unter M365 Compliance > **Einstellungen** vermissen, überprüfen Sie, ob Sie über die entsprechende Lizenz und die entsprechenden Berechtigungen verfügen, auf die oben verwiesen wird.</span><span class="sxs-lookup"><span data-stu-id="f6cb0-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="f6cb0-114">Weitere Informationen finden Sie unter [Onboarding von Geräten](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="f6cb0-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="f6cb0-115">Erstellen Sie DLP-Richtlinien zum Schutz Ihrer vertraulichen Elemente.</span><span class="sxs-lookup"><span data-stu-id="f6cb0-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="f6cb0-116">Informationen hierzu finden Sie unter [Szenarien für Endpunkt-DLP-Richtlinien](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="f6cb0-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="f6cb0-117">Weitere Informationen zu Microsoft Endpunkt-DLP finden Sie unter [Informationen zu Microsoft 365 Endpunkt-DLP (Data Loss Prevention, Verhinderung von Datenverlust) (Vorschau)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="f6cb0-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="f6cb0-118">**Wichtige Datenerfassungsschritte, falls Support benötigt wird:**</span><span class="sxs-lookup"><span data-stu-id="f6cb0-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="f6cb0-119">MDATP Client Analyzer-Vorschauversion von [http://aka.ms/betamdatpanalyzer](http://aka.ms/betamdatpanalyzer "http://aka.ms/betamdatpanalyzer") herunterladen</span><span class="sxs-lookup"><span data-stu-id="f6cb0-119">Download MDATP Client Analyzer Preview from [http://aka.ms/betamdatpanalyzer](http://aka.ms/betamdatpanalyzer "http://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="f6cb0-120">Führen Sie das Tool über das CMD-Fenster als Administrator aus:</span><span class="sxs-lookup"><span data-stu-id="f6cb0-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="f6cb0-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="f6cb0-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="f6cb0-122">Wenn Sie mit "Geben Sie die Anzahl der Minuten ein, in denen die Ablaufverfolgungen erfasst werden soll" aufgefordert werden, geben Sie Dauer, die für die Ausführung des Szenarios erforderlich ist, in Minuten ein.</span><span class="sxs-lookup"><span data-stu-id="f6cb0-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="f6cb0-123">Ausführen des Szenarios</span><span class="sxs-lookup"><span data-stu-id="f6cb0-123">Run the scenario</span></span>

<span data-ttu-id="f6cb0-124">Erfassen Sie die ZIP-Dateiausgabe, um sie dem Supportmitarbeiter zu übergeben.</span><span class="sxs-lookup"><span data-stu-id="f6cb0-124">Collect the Zip file output to be given to the Support agent.</span></span>
