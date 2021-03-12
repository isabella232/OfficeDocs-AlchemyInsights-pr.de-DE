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
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708673"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="9082b-102">Überwachen des bedingten Zugriffs für Exchange</span><span class="sxs-lookup"><span data-stu-id="9082b-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="9082b-103">Benutzer mit bedingten Zugriff erhalten eine Benachrichtigungs-E-Mail, wenn sie die Zugriffsanforderungen Ihrer Organisation nicht erfüllen.</span><span class="sxs-lookup"><span data-stu-id="9082b-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="9082b-104">Zur Lösung empfehlen wir eine oder mehrere der folgenden Lösungen:</span><span class="sxs-lookup"><span data-stu-id="9082b-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="9082b-105">Wenn angenommen wird, dass das Gerät registriert ist, empfehlen Sie dem Benutzer, zur Unternehmensportal-App zu wechseln und zu überprüfen, ob es im Unternehmensportal angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="9082b-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="9082b-106">Andern falls nicht, sollte der Benutzer das Gerät registrieren.</span><span class="sxs-lookup"><span data-stu-id="9082b-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="9082b-107">Wechseln Sie im Azure-Portal zu Intune > Gerätekonformität.</span><span class="sxs-lookup"><span data-stu-id="9082b-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="9082b-108">Klicken Sie unter Überwachen auf Gerätekonformität.</span><span class="sxs-lookup"><span data-stu-id="9082b-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="9082b-109">Zeigen Sie den Bericht zur Gerätekonformität an, um zu überprüfen, ob das Gerät des Benutzers als kompatibel gekennzeichnet ist.</span><span class="sxs-lookup"><span data-stu-id="9082b-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="9082b-110">Wechseln Sie im Azure-Portal zu Intune > Gerätekonformität.</span><span class="sxs-lookup"><span data-stu-id="9082b-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="9082b-111">Klicken Sie unter Verwalten auf Richtlinien.</span><span class="sxs-lookup"><span data-stu-id="9082b-111">Under Manage, click Policies.</span></span> <span data-ttu-id="9082b-112">Überprüfen Sie in der Liste der Compliancerichtlinien, ob dem Gerät Ihres Benutzers ein Profil zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="9082b-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="9082b-113">Wenn kein Profil zugewiesen ist, kann Intune den Kompatibilitätsstatus des Geräts nicht bestätigen.</span><span class="sxs-lookup"><span data-stu-id="9082b-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="9082b-114">Bearbeiten Sie die Zuweisung für bedingten Zugriff des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="9082b-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="9082b-115">Wechseln Sie im Azure-Portal zu  >  **Intune-Richtlinien für bedingten**  >  **Zugriff.**</span><span class="sxs-lookup"><span data-stu-id="9082b-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="9082b-116">Wählen Sie eine Richtlinie aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="9082b-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="9082b-117">Klicken Sie auf Benutzer und Gruppen.</span><span class="sxs-lookup"><span data-stu-id="9082b-117">Click Users and groups.</span></span>
4. <span data-ttu-id="9082b-118">Um eine bestimmte Richtlinie auf eine Person zu zielen, fügen Sie sie der Include-Liste hinzu.</span><span class="sxs-lookup"><span data-stu-id="9082b-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="9082b-119">Um sicherzustellen, dass eine Person aus der Richtlinie ausgelassen wird, fügen Sie sie der Liste Ausschließen hinzu.</span><span class="sxs-lookup"><span data-stu-id="9082b-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="9082b-120">Hilfreiche Links:</span><span class="sxs-lookup"><span data-stu-id="9082b-120">Helpful links:</span></span>

[<span data-ttu-id="9082b-121">Übersicht über die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="9082b-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="9082b-122">Problembehandlung bei der Zertifizierungsstelle</span><span class="sxs-lookup"><span data-stu-id="9082b-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="9082b-123">Problembehandlungsrichtlinie</span><span class="sxs-lookup"><span data-stu-id="9082b-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="9082b-124">Überwachen der Intune-Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="9082b-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="9082b-125">Hinweis: Diese Schritte sind nur bei der Problembehandlung für das Azure Active Directory-Feature Bedingter Zugriff hilfreich.</span><span class="sxs-lookup"><span data-stu-id="9082b-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="9082b-126">Es ist auch möglich, ein Gerät unter Quarantäne zu stellen, das den E-Mail-Zugriff mit der Exchange-Richtlinie blockiert.</span><span class="sxs-lookup"><span data-stu-id="9082b-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="9082b-127">Weitere Informationen zur Exchange-Geräteverwaltung finden Sie [hier]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="9082b-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
