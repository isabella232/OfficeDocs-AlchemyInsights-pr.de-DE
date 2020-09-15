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
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702902"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="0a702-102">Überwachen des bedingten Zugriffs für Exchange</span><span class="sxs-lookup"><span data-stu-id="0a702-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="0a702-103">Benutzer, die auf bedingten Zugriff abzielen, erhalten eine Benachrichtigungs-e-Mail, wenn Sie die Zugriffsanforderungen Ihrer Organisation nicht erfüllen.</span><span class="sxs-lookup"><span data-stu-id="0a702-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="0a702-104">Zur Behebung empfehlen wir eine oder mehrere der folgenden Lösungen:</span><span class="sxs-lookup"><span data-stu-id="0a702-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="0a702-105">Wenn Sie davon ausgehen, dass das Gerät registriert ist, empfehlen Sie dem Benutzer, zur Unternehmensportal-APP zu wechseln und zu überprüfen, ob er im Unternehmensportal angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="0a702-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="0a702-106">Wenn dies nicht der Fall ist, sollte der Benutzer das Gerät registrieren.</span><span class="sxs-lookup"><span data-stu-id="0a702-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="0a702-107">Wechseln Sie im Azure-Portal zu **InTune- \> Gerätekompatibilität**.</span><span class="sxs-lookup"><span data-stu-id="0a702-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="0a702-108">Klicken Sie unter **Überwachung** auf **Gerätekompatibilität**.</span><span class="sxs-lookup"><span data-stu-id="0a702-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="0a702-109">Zeigen Sie Ihren Geräte Kompatibilitätsbericht an, um zu überprüfen, ob das Gerät des Benutzers als konform gekennzeichnet ist.</span><span class="sxs-lookup"><span data-stu-id="0a702-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="0a702-110">Wechseln Sie im Azure-Portal zu **InTune- \> Gerätekompatibilität**.</span><span class="sxs-lookup"><span data-stu-id="0a702-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="0a702-111">Klicken Sie unter **Verwalten**auf **Richtlinien**.</span><span class="sxs-lookup"><span data-stu-id="0a702-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="0a702-112">Überprüfen Sie in der Liste der Konformitätsrichtlinien, ob ein Profil dem Gerät Ihres Benutzers zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="0a702-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="0a702-113">Wenn kein Profil zugewiesen ist, kann InTune den Kompatibilitätsstatus des Geräts nicht bestätigen.</span><span class="sxs-lookup"><span data-stu-id="0a702-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="0a702-114">Bearbeiten Sie die Zuweisung für bedingten Zugriff des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="0a702-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="0a702-115">Im Azure-Portal gehen Sie zu **InTune- \> \> Richtlinien für bedingten Zugriff**</span><span class="sxs-lookup"><span data-stu-id="0a702-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="0a702-116">Auswählen einer Richtlinie aus der Liste</span><span class="sxs-lookup"><span data-stu-id="0a702-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="0a702-117">Klicken Sie auf **Benutzer und Gruppen** .</span><span class="sxs-lookup"><span data-stu-id="0a702-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="0a702-118">Um eine bestimmte Richtlinie auf eine Person abzuzielen, fügen Sie Sie der Liste **einschließen** hinzu.</span><span class="sxs-lookup"><span data-stu-id="0a702-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="0a702-119">Um sicherzustellen, dass eine Person aus der Richtlinie weggelassen wird, fügen Sie Sie der **Ausschluss** Liste hinzu.</span><span class="sxs-lookup"><span data-stu-id="0a702-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="0a702-120">Weitere Informationen: [Vorgehensweise zum Überwachen von bedingten Zugriffs Geräten](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="0a702-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

