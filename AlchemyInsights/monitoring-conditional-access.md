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
# <a name="monitoring-conditional-access"></a>ÜberWachen des bedingten Zugriffs

Benutzer mit bedingtem Zugriff erhalten eine Benachrichtigungs-e-Mail, wenn Sie die Zugriffsanforderungen Ihrer Organisation nicht erfüllen. Zur Lösung empfehlen wir eine oder mehrere der folgenden Lösungen:
  
- Wenn das Gerät als registriert gilt, empfehlen Sie dem Benutzer, zur Unternehmensportal-APP zu wechseln und sicherzustellen, dass es im Unternehmensportal angezeigt wird. Wenn dies nicht der Fall ist, sollte der Benutzer das Gerät registrieren.
    
- Wechseln Sie im Azure-Portal **zu \> InTune Device Compliance**. Klicken Sie unter **Monitor** auf **Geräte Konformität**. Zeigen Sie Ihren Geräte Konformitätsbericht an, um zu überprüfen, ob das Gerät des Benutzers als kompatibel gekennzeichnet ist. 
    
- Wechseln Sie im Azure-Portal **zu \> InTune Device Compliance**. Klicken Sie unter **Verwalten**auf **Richtlinien**. Vergewissern Sie sich in der Liste der Konformitätsrichtlinien, dass dem Gerät des Benutzers ein Profil zugewiesen ist. Wenn kein Profil zugewiesen ist, kann InTune den Kompatibilitätsstatus des Geräts nicht bestätigen. 
    
- Bearbeiten Sie die Zuweisung des bedingten Zugriffs durch den Benutzer.
    
1. Navigieren Sie im Azure-Portal **zu \> InTune- \> Richtlinien für bedingten Zugriff** .
    
2. Wählen Sie eine Richtlinie aus der Liste aus.
    
3. Klicken Sie auf **Benutzer und Gruppen**
    
4. Wenn Sie eine bestimmte Richtlinie auf eine andere Person anwenden möchten **** , fügen Sie Sie der Liste include hinzu. Um sicherzustellen, dass eine Person in der Richtlinie ausgelassen wird, fügen Sie Sie der **Ausschluss** Liste hinzu. 
    
Weitere Informationen: [so ÜberwachEn Sie Geräte für bedingten Zugriff](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

