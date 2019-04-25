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
# <a name="working-with-ios-vpp-applications"></a>Arbeiten mit iOS-VPP-Anwendungen

Hier erfahren Sie, [wie Sie IOS-apps verwalten, die über ein Volume-Purchase-Programm mit Microsoft InTune erworben](https://docs.microsoft.com/intune/vpp-apps-ios) wurden, um mehr über Features, Einschränkungen und Schritte zur Verwendung des Apple Volume Purchase-Programms und die Unterstützung für IT in Microsoft InTune zu lernen. 
  
 **Häufige Probleme:** "Ich habe meinen Benutzern eine iOS VSS-App zugewiesen, aber die Installation ist fehlgeschlagen." 
  
- Dies kann passieren, wenn ein einzelnes VSS-Token über mehrere Verwaltungsanbieter für mobile Geräte verwendet wird. VPP-Token von Apple dürfen nur mit einem Anbieter verwendet werden. Wenn Sie ein VPP-Token mit mehreren Anbietern verwendet haben, müssen Sie das Token erneut in InTune hochladen.
    
- Die Installation kann auch fehlschlagen, wenn die Gesamtzahl der Installationen die Anzahl der Lizenzen überschreitet. Um einen Verwendungsbericht für Ihre Lizenzen anzuzeigen, wechseln Sie zur Seite " **InTune Mobile Apps** \> **App licenses** ". Informationen dazu, wie Sie verwendete Lizenzen wieder anfordern können, finden Sie in [diesem Artikel.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
    

