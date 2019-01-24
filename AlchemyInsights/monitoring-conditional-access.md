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
# <a name="monitoring-conditional-access"></a>Überwachen von bedingten Zugriff

Benutzer mit bedingten Zugriff zielorientierten erhält eine e-Mail-Benachrichtigung, wenn sie keine Access-Anforderungen Ihrer Organisation entsprechen. Um zu beheben, empfehlen wir eine oder mehrere der folgenden Lösungen:
  
- Das Gerät für registriert werden vermutet wird, informieren des Benutzers wechseln zu der app Unternehmensportal und stellen Sie sicher, dass es im Unternehmensportal angezeigt wird. Wenn dies nicht der Fall, sollte der Benutzer das Gerät zu registrieren.
    
- Wechseln Sie im Azure-Portal zur **Intune \> Gerät Compliance**. Klicken Sie unter **Monitor** auf **Gerät Compliance**. Zeigen Sie Ihres Berichts Gerät Compliance, um sicherzustellen, dass das Gerät des Benutzers als kompatibel markiert ist an. 
    
- Wechseln Sie im Azure-Portal zur **Intune \> Gerät Compliance**. Klicken Sie unter **Verwalten**auf **Richtlinien**. In der Liste der Richtlinien für die Kompatibilität stellen Sie sicher, dass das Gerät des Benutzers ein Profil zugewiesen ist. Wenn kein Profil zugewiesen ist, klicken Sie dann werden Intune können Sie überprüfen, das Gerät Kompatibilitätsstatus nicht. 
    
- Bearbeiten des Benutzers bedingte Access-Zuordnung.
    
1. Wechseln Sie im Azure-Portal zur **Intune \> bedingten Zugriff \> Richtlinien**
    
2. Wählen Sie eine Richtlinie aus der Liste aus.
    
3. Klicken Sie auf **Benutzer und Gruppen**
    
4. Um eine bestimmte Richtlinie an eine Person zu entwickeln, fügen sie Sie **der Liste** hinzu. Um sicherzustellen, dass eine Person aus der Richtlinie ausgelassen wird, fügen sie **der Ausschlussliste** hinzu. 
    
Weitere: [wie bedingte Zugriff überwachen Geräte](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)
  

