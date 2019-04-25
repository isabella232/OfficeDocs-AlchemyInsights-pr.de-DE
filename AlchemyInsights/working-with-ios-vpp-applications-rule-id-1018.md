---
title: Arbeiten mit der iOS-VPP-Anwendung Regel-ID 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420483"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="4b368-102">Arbeiten mit iOS-VPP-Anwendungen</span><span class="sxs-lookup"><span data-stu-id="4b368-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="4b368-103">Hier erfahren Sie, [wie Sie IOS-apps verwalten, die über ein Volume-Purchase-Programm mit Microsoft InTune erworben](https://docs.microsoft.com/intune/vpp-apps-ios) wurden, um mehr über Features, Einschränkungen und Schritte zur Verwendung des Apple Volume Purchase-Programms und die Unterstützung für IT in Microsoft InTune zu lernen.</span><span class="sxs-lookup"><span data-stu-id="4b368-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="4b368-104">**Häufige Probleme:** "Ich habe meinen Benutzern eine iOS VSS-App zugewiesen, aber die Installation ist fehlgeschlagen."</span><span class="sxs-lookup"><span data-stu-id="4b368-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="4b368-105">Dies kann passieren, wenn ein einzelnes VSS-Token über mehrere Verwaltungsanbieter für mobile Geräte verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="4b368-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="4b368-106">VPP-Token von Apple dürfen nur mit einem Anbieter verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="4b368-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="4b368-107">Wenn Sie ein VPP-Token mit mehreren Anbietern verwendet haben, müssen Sie das Token erneut in InTune hochladen.</span><span class="sxs-lookup"><span data-stu-id="4b368-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="4b368-108">Die Installation kann auch fehlschlagen, wenn die Gesamtzahl der Installationen die Anzahl der Lizenzen überschreitet.</span><span class="sxs-lookup"><span data-stu-id="4b368-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="4b368-109">Um einen Verwendungsbericht für Ihre Lizenzen anzuzeigen, wechseln Sie zur Seite " **InTune Mobile Apps** \> **App licenses** ".</span><span class="sxs-lookup"><span data-stu-id="4b368-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="4b368-110">Informationen dazu, wie Sie verwendete Lizenzen wieder anfordern können, finden Sie in [diesem Artikel.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="4b368-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

