---
title: Website-Ermittlung durchführen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529228"
---
# <a name="do-site-discovery"></a><span data-ttu-id="21da1-102">Website-Ermittlung durchführen</span><span class="sxs-lookup"><span data-stu-id="21da1-102">Do site discovery</span></span>

<span data-ttu-id="21da1-103">Falls in Ihrer Organisation noch ältere Webanwendungen genutzt werden und die Verwendung des Internet Explorer-Modus geplant ist (was auf die meisten Kunden zutrifft), sollten Sie etwas zusätzliche Website-Ermittlung durchführen.</span><span class="sxs-lookup"><span data-stu-id="21da1-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="21da1-104">**Sie haben bereits eine ältere Version von Microsoft Edge bereitgestellt**</span><span class="sxs-lookup"><span data-stu-id="21da1-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="21da1-105">Wenn Sie Ihre Enterprise-Websiteliste bereits für die ältere Version von Microsoft Edge konfiguriert haben, ist die Website-Ermittlung fast abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="21da1-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="21da1-106">Wahrscheinlich müssen Sie nur noch neutrale Websites hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="21da1-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="21da1-107">Neutrale Websites sind in der Regel Websites, die einmaliges Anmelden (Single Sign-On, SSO) bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="21da1-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="21da1-108">Wenn Sie zu einer neutralen Website über Microsoft Edge wechseln, möchten Sie zur Authentifizierung in Microsoft Edge bleiben.</span><span class="sxs-lookup"><span data-stu-id="21da1-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="21da1-109">Wenn Sie im Internet Explorer-Modus zu einer neutralen Website wechseln, möchten Sie zur Authentifizierung im Internet Explorer-Modus bleiben.</span><span class="sxs-lookup"><span data-stu-id="21da1-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="21da1-110">Ermitteln Sie alle SSO- oder andere neutrale Websites, die Sie verwenden, und fügen Sie diese Ihrer Enterprise-Websiteliste hinzu.</span><span class="sxs-lookup"><span data-stu-id="21da1-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="21da1-111">**Internet Explorer ist Ihr Standardbrowser**</span><span class="sxs-lookup"><span data-stu-id="21da1-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="21da1-112">Wenn Sie derzeit nur Internet Explorer verwenden, wissen Sie möglicherweise nicht, welche Websites auf moderne Webstandards aktualisiert wurden, und für welche weiterhin Internet Explorer erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="21da1-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="21da1-113">Sie sollten diese Websites ermitteln und der Enterprise-Websiteliste hinzufügen, damit der Internet Explorer-Modus nur für diese Websites verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="21da1-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="21da1-114">Bei der [Enterprise-Website-Ermittlung](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) werden Websites ermittelt, für die möglicherweise der Internet Explorer-Modus benötigt wird.</span><span class="sxs-lookup"><span data-stu-id="21da1-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="21da1-115">Dabei können Daten auf Computern mit Windows Internet Explorer 8 bis Internet Explorer 11 unter Windows 10, Windows 8.1 oder Windows 7 erfasst werden.</span><span class="sxs-lookup"><span data-stu-id="21da1-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="21da1-116">**Analysieren der Daten**</span><span class="sxs-lookup"><span data-stu-id="21da1-116">**Analyze the data**</span></span>

<span data-ttu-id="21da1-117">Nach deren Erfassung empfehlen wir die folgenden vier Schritte zum Analysieren der Daten:</span><span class="sxs-lookup"><span data-stu-id="21da1-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="21da1-118">Sortieren Sie die Daten nach Domäne und dann nach URL.</span><span class="sxs-lookup"><span data-stu-id="21da1-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="21da1-119">Definieren Sie die Grenzen einer App, die für den Internet Explorer-Modus konfiguriert werden soll.</span><span class="sxs-lookup"><span data-stu-id="21da1-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="21da1-120">Ihr Ziel ist es, alle Websites und Websteuerelemente, die die App definieren, einzuschließen, jedoch keine zusätzlichen Websites und Steuerelemente.</span><span class="sxs-lookup"><span data-stu-id="21da1-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="21da1-121">Einige Sites sind möglicherweise so einfach wie *https://contoso.com/app1*, während andere möglicherweise erfordern, dass Sie mehrere Websites und Seiten definieren.</span><span class="sxs-lookup"><span data-stu-id="21da1-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="21da1-122">Testen Sie die App, um zu verifizieren, dass sie nicht nativ funktioniert.</span><span class="sxs-lookup"><span data-stu-id="21da1-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="21da1-123">Viele Websites stellen modernen Inhalt bereit, wenn sie einen modernen Browser erkennen, und älteren, wenn sie Internet Explorer erkennen.</span><span class="sxs-lookup"><span data-stu-id="21da1-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="21da1-124">Fügen Sie die App Ihrer Enterprise-Websiteliste hinzu, wenn der Test fehlschlägt.</span><span class="sxs-lookup"><span data-stu-id="21da1-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="21da1-125">Eine bewährte Methode beseht darin, alle Websites, die eine App umfassen, zu gruppieren.</span><span class="sxs-lookup"><span data-stu-id="21da1-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="21da1-126">Auf diese Weise ist es einfacher, die gesamte Website aus dem Internet Explorer-Modus zu entfernen, wenn Sie ein Upgrade einer App durchführen, und mit der Verwendung eines modernen Browsers für diese App zu beginnen.</span><span class="sxs-lookup"><span data-stu-id="21da1-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="21da1-127">Nachdem Sie die Website-Ermittlung durchgeführt und die Daten analysiert haben, können Sie sich mit Ihrer Kanalstrategie befassen.</span><span class="sxs-lookup"><span data-stu-id="21da1-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

