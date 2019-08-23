---
title: Arbeiten mit IOS VPP-Anwendungen Regelkennung 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: a0bbc1f49f251ef4f16300c8cca98e219008d17e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36557993"
---
# <a name="working-with-ios-vpp-applications"></a>Arbeiten mit IOS-VPP-Anwendungen

In diesem Artikel erfahren Sie, [wie Sie IOS-apps verwalten können, die über ein Volumen Einkaufsprogramm mit Microsoft InTune erworben](https://docs.microsoft.com/intune/vpp-apps-ios) wurden, um sich über Features, Einschränkungen und Schritte für die Verwendung des Apple Volume Purchase-Programms und dessen Unterstützung in Microsoft InTune zu informieren.
  
 **Häufige Probleme:** "Ich habe meinen Benutzern eine IOS VPP-App zugewiesen, aber die Installation ist fehlgeschlagen."
  
- Dies kann vorkommen, wenn ein einzelnes VPP-Token für mehrere Anbieter für die Verwaltung mobiler Geräte verwendet wird. VPP-Token von Apple dürfen nur mit einem Anbieter verwendet werden. Wenn Sie ein VPP-Token mit mehreren Anbietern verwendet haben, müssen Sie das Token erneut in InTune hochladen.

- Die Installation kann auch fehlschlagen, wenn die Gesamtanzahl der Installationen die Anzahl der Lizenzen überschreitet. Um einen Verwendungsbericht für Ihre Lizenzen anzuzeigen, wechseln Sie zur Seite **InTune Mobile Apps** \> - **App-Lizenzen** . Informationen zum Freigeben von Lizenzen in use finden Sie in [diesem Artikel.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
