---
title: Überwachen des bedingten Zugriffs
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366427"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="7852a-102">Überwachen des bedingten Zugriffs für Exchange</span><span class="sxs-lookup"><span data-stu-id="7852a-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="7852a-103">Benutzer, die auf bedingten Zugriff abzielen, erhalten eine Benachrichtigungs-e-Mail, wenn Sie die Zugriffsanforderungen Ihrer Organisation nicht erfüllen.</span><span class="sxs-lookup"><span data-stu-id="7852a-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="7852a-104">Zur Behebung empfehlen wir eine oder mehrere der folgenden Lösungen:</span><span class="sxs-lookup"><span data-stu-id="7852a-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="7852a-105">Wenn Sie davon ausgehen, dass das Gerät registriert ist, empfehlen Sie dem Benutzer, zur Unternehmensportal-APP zu wechseln und zu überprüfen, ob er im Unternehmensportal angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="7852a-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="7852a-106">Wenn dies nicht der Fall ist, sollte der Benutzer das Gerät registrieren.</span><span class="sxs-lookup"><span data-stu-id="7852a-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="7852a-107">Wechseln Sie im Azure-Portal zu InTune-> Gerätekompatibilität.</span><span class="sxs-lookup"><span data-stu-id="7852a-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="7852a-108">Klicken Sie unter Überwachung auf Gerätekompatibilität.</span><span class="sxs-lookup"><span data-stu-id="7852a-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="7852a-109">Zeigen Sie Ihren Geräte Kompatibilitätsbericht an, um zu überprüfen, ob das Gerät des Benutzers als konform gekennzeichnet ist.</span><span class="sxs-lookup"><span data-stu-id="7852a-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="7852a-110">Wechseln Sie im Azure-Portal zu InTune-> Gerätekompatibilität.</span><span class="sxs-lookup"><span data-stu-id="7852a-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="7852a-111">Klicken Sie unter Verwalten auf Richtlinien.</span><span class="sxs-lookup"><span data-stu-id="7852a-111">Under Manage, click Policies.</span></span> <span data-ttu-id="7852a-112">Überprüfen Sie in der Liste der Konformitätsrichtlinien, ob ein Profil dem Gerät Ihres Benutzers zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="7852a-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="7852a-113">Wenn kein Profil zugewiesen ist, kann InTune den Kompatibilitätsstatus des Geräts nicht bestätigen.</span><span class="sxs-lookup"><span data-stu-id="7852a-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="7852a-114">Bearbeiten Sie die Zuweisung für bedingten Zugriff des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="7852a-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="7852a-115">Navigieren Sie im Azure-Portal zu **InTune**  >  **Conditional access**  >  -**Richtlinien**für bedingten Zugriff.</span><span class="sxs-lookup"><span data-stu-id="7852a-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="7852a-116">Wählen Sie eine Richtlinie aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="7852a-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="7852a-117">Klicken Sie auf Benutzer und Gruppen.</span><span class="sxs-lookup"><span data-stu-id="7852a-117">Click Users and groups.</span></span>
4. <span data-ttu-id="7852a-118">Um eine bestimmte Richtlinie auf eine Person abzuzielen, fügen Sie Sie der Liste einschließen hinzu.</span><span class="sxs-lookup"><span data-stu-id="7852a-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="7852a-119">Um sicherzustellen, dass eine Person aus der Richtlinie weggelassen wird, fügen Sie Sie der Ausschlussliste hinzu.</span><span class="sxs-lookup"><span data-stu-id="7852a-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="7852a-120">Hilfreiche Links:</span><span class="sxs-lookup"><span data-stu-id="7852a-120">Helpful links:</span></span>

[<span data-ttu-id="7852a-121">Übersicht über die Gerätekompatibilität</span><span class="sxs-lookup"><span data-stu-id="7852a-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="7852a-122">Problembehandlung bei ca</span><span class="sxs-lookup"><span data-stu-id="7852a-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="7852a-123">Problem behandlungsrichtlinie</span><span class="sxs-lookup"><span data-stu-id="7852a-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="7852a-124">Überwachen der InTune-Gerätekompatibilität</span><span class="sxs-lookup"><span data-stu-id="7852a-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="7852a-125">Hinweis: diese Schritte sind nur hilfreich bei der Problembehandlung für den bedingten Zugriff auf Azure Active Directory Feature.</span><span class="sxs-lookup"><span data-stu-id="7852a-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="7852a-126">Es ist auch möglich, ein Gerät zu isolieren, das den e-Mail-Zugriff mit der Exchange-Richtlinie blockiert.</span><span class="sxs-lookup"><span data-stu-id="7852a-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="7852a-127">Weitere Informationen zur Exchange-Geräteverwaltung finden Sie [hier](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span><span class="sxs-lookup"><span data-stu-id="7852a-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
