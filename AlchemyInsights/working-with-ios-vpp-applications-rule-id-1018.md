---
title: Arbeiten mit iOS VPP Applications Regel-Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 5bcfb6dd7222bd102ff2620c19bfb943e7bd9591
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29470149"
---
# <a name="working-with-ios-vpp-applications"></a>Arbeiten mit iOS VPP Applikationen

Hier erhalten Sie [zur Verwaltung von iOS-apps, die über ein Programm Volume Purchase mit Microsoft Intune erworben](https://docs.microsoft.com/intune/vpp-apps-ios) Weitere Informationen zu Features, Einschränkungen und Schritte zum Erstellen des Apple Volume erwerben Programms und Support für Microsoft Intune verwenden. 
  
 **Häufig auftretender Probleme:** "Meine Benutzer eine app für iOS VPP zugewiesen, aber die Installation ist fehlgeschlagen." 
  
- Dies kann vorkommen, wenn ein einzelnes Token VPP über mehrere Mobilgerät Management-Anbieter verwendet wird. VPP Tokens von Apple können nur mit einem Anbieter verwendet werden. Wenn Sie ein Token VPP mit mehreren Anbietern verwendet, müssen Sie das Token fest Intune erneut hochladen.
    
- Die Installation kann auch fehl, wenn die Gesamtanzahl der Installationen die Anzahl der Lizenzen überschreiten. Einen Verwendungsbericht für Ihre Lizenzen wechseln Sie zum Anzeigen der **Intune Mobile apps** \> Seite **App-Lizenzen** . Informationen zum Freigeben von Lizenzen verwendet, finden Sie unter [in diesem Artikel.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
    

