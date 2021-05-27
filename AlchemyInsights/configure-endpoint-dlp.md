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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657928"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="0a65f-102">Konfigurieren von Endpunkt-DLP</span><span class="sxs-lookup"><span data-stu-id="0a65f-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="0a65f-103">Microsoft Endpunkt-DLP bietet Ihnen die Möglichkeit, Schutz- und Überwachungsfunktionen von DLP auf vertrauliche Informationen auf Windows 10-Geräten zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="0a65f-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="0a65f-104">Nachdem die Geräte in die Geräteverwaltung integriert wurden, können Sie DLP-Richtlinien erstellen, um Schutzmaßnahmen für Objekte durchzusetzen.</span><span class="sxs-lookup"><span data-stu-id="0a65f-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="0a65f-105">Der Aktivitäten-Explorer kann verwendet werden, um die Aktivität für vertrauliche Elemente zu überwachen.</span><span class="sxs-lookup"><span data-stu-id="0a65f-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="0a65f-106">Weitere Informationen finden Sie unter [Onboarding von Geräten für die Geräteverwaltung](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="0a65f-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="0a65f-107">So führen Sie die ersten Schritte mit Endpunkt-DLP aus</span><span class="sxs-lookup"><span data-stu-id="0a65f-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="0a65f-108">Stellen Sie sicher, dass Sie über die geeignete SKU/Abonnementlizenzierung verfügen.</span><span class="sxs-lookup"><span data-stu-id="0a65f-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="0a65f-109">Weitere Informationen finden Sie unter [SKU/Abonnement-Lizenzierung](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="0a65f-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="0a65f-110">Überprüfen Sie die Berechtigungen, die erforderlich sind, um die Geräteverwaltung zu aktivieren, auf die Onboardingseite zuzugreifen oder die Geräteüberwachung ein- und auszuschalten.</span><span class="sxs-lookup"><span data-stu-id="0a65f-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="0a65f-111">Weitere Informationen finden Sie unter [Berechtigungen](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="0a65f-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="0a65f-112">Führen Sie ein Onboarding der Geräte in die Geräteverwaltung aus, indem Sie dem Verfahren für das Onboarding von Geräten folgen.</span><span class="sxs-lookup"><span data-stu-id="0a65f-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="0a65f-113">Weitere Informationen finden Sie unter [Onboarding von Geräten](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="0a65f-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="0a65f-114">Erstellen Sie DLP-Richtlinien zum Schutz Ihrer vertraulichen Elemente.</span><span class="sxs-lookup"><span data-stu-id="0a65f-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="0a65f-115">Informationen hierzu finden Sie unter [Szenarien für Endpunkt-DLP-Richtlinien](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="0a65f-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="0a65f-116">Weitere Informationen zu Microsoft Endpunkt-DLP finden Sie unter [Informationen zu Microsoft 365 Endpunkt-DLP (Data Loss Prevention, Verhinderung von Datenverlust) (Vorschau)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="0a65f-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="0a65f-117">**Wichtige Datenerfassungsschritte, falls Support benötigt wird:**</span><span class="sxs-lookup"><span data-stu-id="0a65f-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="0a65f-118">[MDATP Client Analyzer-Vorschauversion](https://aka.ms/betamdatpanalyzer) herunterladen.</span><span class="sxs-lookup"><span data-stu-id="0a65f-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="0a65f-119">Führen Sie das Tool über das CMD-Fenster als Administrator aus:</span><span class="sxs-lookup"><span data-stu-id="0a65f-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="0a65f-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="0a65f-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="0a65f-121">Wenn Sie mit **Geben Sie die Anzahl der Minuten ein, in denen die Ablaufverfolgungen erfasst werden soll** aufgefordert werden, geben Sie Dauer, die für die Ausführung des Szenarios erforderlich ist, in Minuten ein.</span><span class="sxs-lookup"><span data-stu-id="0a65f-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="0a65f-122">Führen Sie das Szenario aus.</span><span class="sxs-lookup"><span data-stu-id="0a65f-122">Run the scenario.</span></span>

<span data-ttu-id="0a65f-123">Erfassen Sie die ZIP-Dateiausgabe, um sie dem Supportmitarbeiter zu übergeben.</span><span class="sxs-lookup"><span data-stu-id="0a65f-123">Collect the Zip file output to give to the Support agent.</span></span>
