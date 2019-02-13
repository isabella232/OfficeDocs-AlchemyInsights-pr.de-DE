---
title: Arbeiten mit iOS VPP Applications Regel-Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917495"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="352dc-102">Arbeiten mit iOS VPP Applikationen</span><span class="sxs-lookup"><span data-stu-id="352dc-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="352dc-103">Hier erhalten Sie [zur Verwaltung von iOS-apps, die über ein Programm Volume Purchase mit Microsoft Intune erworben](https://docs.microsoft.com/intune/vpp-apps-ios) Weitere Informationen zu Features, Einschränkungen und Schritte zum Erstellen des Apple Volume erwerben Programms und Support für Microsoft Intune verwenden.</span><span class="sxs-lookup"><span data-stu-id="352dc-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="352dc-104">**Häufig auftretender Probleme:** "Meine Benutzer eine app für iOS VPP zugewiesen, aber die Installation ist fehlgeschlagen."</span><span class="sxs-lookup"><span data-stu-id="352dc-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="352dc-p101">Dies kann vorkommen, wenn ein einzelnes Token VPP über mehrere Mobilgerät Management-Anbieter verwendet wird. VPP Tokens von Apple können nur mit einem Anbieter verwendet werden. Wenn Sie ein Token VPP mit mehreren Anbietern verwendet, müssen Sie das Token fest Intune erneut hochladen.</span><span class="sxs-lookup"><span data-stu-id="352dc-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="352dc-p102">Die Installation kann auch fehl, wenn die Gesamtanzahl der Installationen die Anzahl der Lizenzen überschreiten. Einen Verwendungsbericht für Ihre Lizenzen wechseln Sie zum Anzeigen der **Intune Mobile apps** \> Seite **App-Lizenzen** . Informationen zum Freigeben von Lizenzen verwendet, finden Sie unter [in diesem Artikel.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="352dc-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

