---
title: Überwachen von bedingten Zugriff
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29469529"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="79ee3-102">Überwachen von bedingten Zugriff</span><span class="sxs-lookup"><span data-stu-id="79ee3-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="79ee3-p101">Benutzer mit bedingten Zugriff zielorientierten erhält eine e-Mail-Benachrichtigung, wenn sie keine Access-Anforderungen Ihrer Organisation entsprechen. Um zu beheben, empfehlen wir eine oder mehrere der folgenden Lösungen:</span><span class="sxs-lookup"><span data-stu-id="79ee3-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="79ee3-p102">Das Gerät für registriert werden vermutet wird, informieren des Benutzers wechseln zu der app Unternehmensportal und stellen Sie sicher, dass es im Unternehmensportal angezeigt wird. Wenn dies nicht der Fall, sollte der Benutzer das Gerät zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="79ee3-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="79ee3-p103">Wechseln Sie im Azure-Portal zur **Intune \> Gerät Compliance**. Klicken Sie unter **Monitor** auf **Gerät Compliance**. Zeigen Sie Ihres Berichts Gerät Compliance, um sicherzustellen, dass das Gerät des Benutzers als kompatibel markiert ist an.</span><span class="sxs-lookup"><span data-stu-id="79ee3-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="79ee3-p104">Wechseln Sie im Azure-Portal zur **Intune \> Gerät Compliance**. Klicken Sie unter **Verwalten**auf **Richtlinien**. In der Liste der Richtlinien für die Kompatibilität stellen Sie sicher, dass das Gerät des Benutzers ein Profil zugewiesen ist. Wenn kein Profil zugewiesen ist, klicken Sie dann werden Intune können Sie überprüfen, das Gerät Kompatibilitätsstatus nicht.</span><span class="sxs-lookup"><span data-stu-id="79ee3-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="79ee3-114">Bearbeiten des Benutzers bedingte Access-Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="79ee3-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="79ee3-115">Wechseln Sie im Azure-Portal zur **Intune \> bedingten Zugriff \> Richtlinien**</span><span class="sxs-lookup"><span data-stu-id="79ee3-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="79ee3-116">Wählen Sie eine Richtlinie aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="79ee3-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="79ee3-117">Klicken Sie auf **Benutzer und Gruppen**</span><span class="sxs-lookup"><span data-stu-id="79ee3-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="79ee3-p105">Um eine bestimmte Richtlinie an eine Person zu entwickeln, fügen sie Sie **der Liste** hinzu. Um sicherzustellen, dass eine Person aus der Richtlinie ausgelassen wird, fügen sie **der Ausschlussliste** hinzu.</span><span class="sxs-lookup"><span data-stu-id="79ee3-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="79ee3-120">Weitere: [wie bedingte Zugriff überwachen Geräte](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="79ee3-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span></span>
  

