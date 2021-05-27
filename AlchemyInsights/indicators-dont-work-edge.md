---
title: Indikatoren funktionieren nicht im Edge-Browser
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/25/2021
ms.locfileid: "52651491"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="19eaf-102">Indikatoren funktionieren nicht im Edge-Browser</span><span class="sxs-lookup"><span data-stu-id="19eaf-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="19eaf-103">Nachdem Sie einen Indikator erstellt haben, wird er von Edge (Smartscreen) nicht mehr unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19eaf-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="19eaf-104">Weitere Informationen finden Sie unter [Erstellen von Indikatoren für IPs und URLs/Domänen](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span><span class="sxs-lookup"><span data-stu-id="19eaf-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="19eaf-105">Schritt 1: Stellen Sie Folgendes sicher</span><span class="sxs-lookup"><span data-stu-id="19eaf-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="19eaf-106">Überprüfen Sie, ob der Indikator richtig ist (keine Tippfehler in IP/URL, richtige Aktion, die richtigen RBAC-Gruppen).</span><span class="sxs-lookup"><span data-stu-id="19eaf-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="19eaf-107">Warten Sie die Mindestdauer von 2 Stunden nach dem Erstellen des Indikators ab, um mögliche Wartezeiten zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="19eaf-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="19eaf-108">Vergewissern Sie sich, dass das System/die Systeme in Microsoft Defender für Endpunkt integriert sind.</span><span class="sxs-lookup"><span data-stu-id="19eaf-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="19eaf-109">Stellen Sie sicher, dass das System/die Systeme mit der Cloud kommunizieren können.</span><span class="sxs-lookup"><span data-stu-id="19eaf-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="19eaf-110">Stellen Sie sicher, dass Smartscreen aktiviert und erreichbar ist, indem Sie zur [Testwebsite](https://demo.smartscreen.msft.net) wechseln.</span><span class="sxs-lookup"><span data-stu-id="19eaf-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="19eaf-111">Schritt 2: Beheben Sie das potenzielle Problem</span><span class="sxs-lookup"><span data-stu-id="19eaf-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="19eaf-112">Stellen Sie sicher, dass der Kunde die Anforderungen erfüllt.</span><span class="sxs-lookup"><span data-stu-id="19eaf-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="19eaf-113">Weitere Details finden Sie unter [Erstellen von Indikatoren für IPs und URLs/Domänen](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span><span class="sxs-lookup"><span data-stu-id="19eaf-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="19eaf-114">Stellen Sie sicher, dass Sie die neueste Version des Edge-Browsers ausführen.</span><span class="sxs-lookup"><span data-stu-id="19eaf-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="19eaf-115">Informationen zur neuesten Version finden Sie unter [Finden Sie heraus, über welche Version von Microsoft Edge Sie verfügen](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span><span class="sxs-lookup"><span data-stu-id="19eaf-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="19eaf-116">Starten Sie den Edge-Browser neu.</span><span class="sxs-lookup"><span data-stu-id="19eaf-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="19eaf-117">Navigieren Sie zur Website, für die Sie einen Indikator eingerichtet haben.</span><span class="sxs-lookup"><span data-stu-id="19eaf-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="19eaf-118">Wenn die Website nicht wie erwartet angezeigt wird, fahren Sie mit Schritt 3 fort.</span><span class="sxs-lookup"><span data-stu-id="19eaf-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="19eaf-119">Schritt 3: Sammeln Sie Daten</span><span class="sxs-lookup"><span data-stu-id="19eaf-119">Step 3: Collect data</span></span>

- <span data-ttu-id="19eaf-120">Sammeln Sie **MDEClientAnalyzer** Diagnosedaten.</span><span class="sxs-lookup"><span data-stu-id="19eaf-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="19eaf-121">Anweisungen finden Sie unter [Probleme beim Onboarding von Microsoft Defender für Endpunkt auf Computern](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="19eaf-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="19eaf-122">Wenn Sie mit dem Installieren und Sammeln einer Fiddler-Ablaufverfolgung vertraut sind, lesen Sie [Telerik Fiddler](http://www.telerik.com/fiddler).</span><span class="sxs-lookup"><span data-stu-id="19eaf-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="19eaf-123">Wenn Sie die Anleitung vom Microsoft-Support bevorzugen, wählen Sie das Supportsymbol unten aus, um einen Support-Fall zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="19eaf-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
