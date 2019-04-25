---
title: ÜberWachen des bedingten Zugriffs
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418468"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="33c75-102">ÜberWachen des bedingten Zugriffs</span><span class="sxs-lookup"><span data-stu-id="33c75-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="33c75-103">Benutzer mit bedingtem Zugriff erhalten eine Benachrichtigungs-e-Mail, wenn Sie die Zugriffsanforderungen Ihrer Organisation nicht erfüllen.</span><span class="sxs-lookup"><span data-stu-id="33c75-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="33c75-104">Zur Lösung empfehlen wir eine oder mehrere der folgenden Lösungen:</span><span class="sxs-lookup"><span data-stu-id="33c75-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="33c75-105">Wenn das Gerät als registriert gilt, empfehlen Sie dem Benutzer, zur Unternehmensportal-APP zu wechseln und sicherzustellen, dass es im Unternehmensportal angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="33c75-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="33c75-106">Wenn dies nicht der Fall ist, sollte der Benutzer das Gerät registrieren.</span><span class="sxs-lookup"><span data-stu-id="33c75-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="33c75-107">Wechseln Sie im Azure-Portal **zu \> InTune Device Compliance**.</span><span class="sxs-lookup"><span data-stu-id="33c75-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="33c75-108">Klicken Sie unter **Monitor** auf **Geräte Konformität**.</span><span class="sxs-lookup"><span data-stu-id="33c75-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="33c75-109">Zeigen Sie Ihren Geräte Konformitätsbericht an, um zu überprüfen, ob das Gerät des Benutzers als kompatibel gekennzeichnet ist.</span><span class="sxs-lookup"><span data-stu-id="33c75-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="33c75-110">Wechseln Sie im Azure-Portal **zu \> InTune Device Compliance**.</span><span class="sxs-lookup"><span data-stu-id="33c75-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="33c75-111">Klicken Sie unter **Verwalten**auf **Richtlinien**.</span><span class="sxs-lookup"><span data-stu-id="33c75-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="33c75-112">Vergewissern Sie sich in der Liste der Konformitätsrichtlinien, dass dem Gerät des Benutzers ein Profil zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="33c75-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="33c75-113">Wenn kein Profil zugewiesen ist, kann InTune den Kompatibilitätsstatus des Geräts nicht bestätigen.</span><span class="sxs-lookup"><span data-stu-id="33c75-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="33c75-114">Bearbeiten Sie die Zuweisung des bedingten Zugriffs durch den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="33c75-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="33c75-115">Navigieren Sie im Azure-Portal **zu \> InTune- \> Richtlinien für bedingten Zugriff** .</span><span class="sxs-lookup"><span data-stu-id="33c75-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="33c75-116">Wählen Sie eine Richtlinie aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="33c75-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="33c75-117">Klicken Sie auf **Benutzer und Gruppen**</span><span class="sxs-lookup"><span data-stu-id="33c75-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="33c75-118">Wenn Sie eine bestimmte Richtlinie auf eine andere Person anwenden möchten \*\*\*\* , fügen Sie Sie der Liste include hinzu.</span><span class="sxs-lookup"><span data-stu-id="33c75-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="33c75-119">Um sicherzustellen, dass eine Person in der Richtlinie ausgelassen wird, fügen Sie Sie der **Ausschluss** Liste hinzu.</span><span class="sxs-lookup"><span data-stu-id="33c75-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="33c75-120">Weitere Informationen: [so ÜberwachEn Sie Geräte für bedingten Zugriff](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="33c75-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

