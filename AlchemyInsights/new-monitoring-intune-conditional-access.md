---
title: Überwachen des bedingten Zugriffs auf Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/03/2021
ms.locfileid: "50417321"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="81ee2-102">Überwachen des bedingten Zugriffs auf Intune</span><span class="sxs-lookup"><span data-stu-id="81ee2-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="81ee2-103">Benutzer mit bedingten Zugriff erhalten eine Benachrichtigungs-E-Mail, wenn sie die Zugriffsanforderungen Ihrer Organisation nicht erfüllen.</span><span class="sxs-lookup"><span data-stu-id="81ee2-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="81ee2-104">Zur Lösung empfehlen wir eine oder mehrere der folgenden Lösungen:</span><span class="sxs-lookup"><span data-stu-id="81ee2-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="81ee2-105">Wenn angenommen wird, dass das Gerät registriert ist, empfehlen Sie dem Benutzer, zur Unternehmensportal-App zu wechseln und zu überprüfen, ob es im Unternehmensportal angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="81ee2-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="81ee2-106">Andern falls nicht, muss der Benutzer das Gerät registrieren.</span><span class="sxs-lookup"><span data-stu-id="81ee2-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="81ee2-107">Wechseln Sie im Azure-Portal zu **Intune**  >  **Device compliance**.</span><span class="sxs-lookup"><span data-stu-id="81ee2-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="81ee2-108">Klicken Sie unter **Überwachen** auf Gerätekonformität, um den Bericht zur Gerätekonformität anzeigen zu können, um zu überprüfen, ob das Gerät des Benutzers als kompatibel **gekennzeichnet ist.**</span><span class="sxs-lookup"><span data-stu-id="81ee2-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="81ee2-109">Wechseln Sie im Azure-Portal zu **Intune**  >  **Device compliance**.</span><span class="sxs-lookup"><span data-stu-id="81ee2-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="81ee2-110">Klicken **Sie unter Verwalten** auf **Richtlinien**.</span><span class="sxs-lookup"><span data-stu-id="81ee2-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="81ee2-111">Überprüfen Sie in der Liste der Compliancerichtlinien, ob dem Gerät Ihres Benutzers ein Profil zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="81ee2-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="81ee2-112">Wenn kein Profil zugewiesen ist, kann Intune den Kompatibilitätsstatus des Geräts nicht bestätigen.</span><span class="sxs-lookup"><span data-stu-id="81ee2-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="81ee2-113">Bearbeiten Sie die Zuweisung für bedingten Zugriff des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="81ee2-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="81ee2-114">Navigieren Sie im Azure-Portal zu   >  **Intune-Richtlinien** für bedingten  >   **Zugriff,** wählen Sie in der Liste eine Richtlinie aus, und klicken Sie auf Benutzer und Gruppen .</span><span class="sxs-lookup"><span data-stu-id="81ee2-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="81ee2-115">Um eine bestimmte Richtlinie auf eine Person zu zielen, fügen Sie sie der **Include-Liste hinzu.**</span><span class="sxs-lookup"><span data-stu-id="81ee2-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="81ee2-116">Um sicherzustellen, dass eine Person aus der Richtlinie ausgelassen wird, fügen Sie sie der **Liste Ausschließen hinzu.**</span><span class="sxs-lookup"><span data-stu-id="81ee2-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="81ee2-117">**Hilfreiche Links:**</span><span class="sxs-lookup"><span data-stu-id="81ee2-117">**Helpful links:**</span></span>

- [<span data-ttu-id="81ee2-118">Übersicht über die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="81ee2-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="81ee2-119">Problembehandlung bei der Zertifizierungsstelle</span><span class="sxs-lookup"><span data-stu-id="81ee2-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="81ee2-120">Problembehandlungsrichtlinie</span><span class="sxs-lookup"><span data-stu-id="81ee2-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="81ee2-121">Überwachen der Intune-Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="81ee2-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="81ee2-122">Diese Schritte sind nur bei der Problembehandlung für das Azure Active Directory-Feature Bedingter Zugriff hilfreich.</span><span class="sxs-lookup"><span data-stu-id="81ee2-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="81ee2-123">Es ist auch möglich, ein Gerät unter Quarantäne zu stellen, das den E-Mail-Zugriff mit der Exchange-Richtlinie blockiert.</span><span class="sxs-lookup"><span data-stu-id="81ee2-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="81ee2-124">Weitere Informationen zur Exchange-Geräteverwaltung finden Sie [**hier**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span><span class="sxs-lookup"><span data-stu-id="81ee2-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
