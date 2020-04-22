---
title: Arbeiten mit IOS VPP-Anwendungen Regelkennung 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719956"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="96944-102">Arbeiten mit IOS-VPP-Anwendungen</span><span class="sxs-lookup"><span data-stu-id="96944-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="96944-103">In diesem Artikel erfahren Sie, [wie Sie IOS-apps verwalten können, die über ein Volumen Einkaufsprogramm mit Microsoft InTune erworben](https://docs.microsoft.com/intune/vpp-apps-ios) wurden, um sich über Features, Einschränkungen und Schritte für die Verwendung des Apple Volume Purchase-Programms und dessen Unterstützung in Microsoft InTune zu informieren.</span><span class="sxs-lookup"><span data-stu-id="96944-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="96944-104">**Häufige Probleme:** "Ich habe meinen Benutzern eine IOS VPP-App zugewiesen, aber die Installation ist fehlgeschlagen."</span><span class="sxs-lookup"><span data-stu-id="96944-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="96944-105">Dies kann vorkommen, wenn ein einzelnes VPP-Token für mehrere Anbieter für die Verwaltung mobiler Geräte verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="96944-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="96944-106">VPP-Token von Apple dürfen nur mit einem Anbieter verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="96944-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="96944-107">Wenn Sie ein VPP-Token mit mehreren Anbietern verwendet haben, müssen Sie das Token erneut in InTune hochladen.</span><span class="sxs-lookup"><span data-stu-id="96944-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="96944-108">Die Installation kann auch fehlschlagen, wenn die Gesamtanzahl der Installationen die Anzahl der Lizenzen überschreitet.</span><span class="sxs-lookup"><span data-stu-id="96944-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="96944-109">Um einen Verwendungsbericht für Ihre Lizenzen anzuzeigen, wechseln Sie zur Seite **InTune Mobile Apps** \> - **App-Lizenzen** .</span><span class="sxs-lookup"><span data-stu-id="96944-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="96944-110">Informationen zum Freigeben von Lizenzen in use finden Sie in [diesem Artikel.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="96944-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
