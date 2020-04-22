---
title: Überwachen des bedingten Zugriffs
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713717"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Überwachen des bedingten Zugriffs für Exchange

Benutzer, die auf bedingten Zugriff abzielen, erhalten eine Benachrichtigungs-e-Mail, wenn Sie die Zugriffsanforderungen Ihrer Organisation nicht erfüllen. Zur Behebung empfehlen wir eine oder mehrere der folgenden Lösungen:
  
- Wenn Sie davon ausgehen, dass das Gerät registriert ist, empfehlen Sie dem Benutzer, zur Unternehmensportal-APP zu wechseln und zu überprüfen, ob er im Unternehmensportal angezeigt wird. Wenn dies nicht der Fall ist, sollte der Benutzer das Gerät registrieren.
    
- Wechseln Sie im Azure-Portal **zu \> InTune-Gerätekompatibilität**. Klicken Sie unter **Überwachung** auf **Gerätekompatibilität**. Zeigen Sie Ihren Geräte Kompatibilitätsbericht an, um zu überprüfen, ob das Gerät des Benutzers als konform gekennzeichnet ist. 
    
- Wechseln Sie im Azure-Portal **zu \> InTune-Gerätekompatibilität**. Klicken Sie unter **Verwalten**auf **Richtlinien**. Überprüfen Sie in der Liste der Konformitätsrichtlinien, ob ein Profil dem Gerät Ihres Benutzers zugewiesen ist. Wenn kein Profil zugewiesen ist, kann InTune den Kompatibilitätsstatus des Geräts nicht bestätigen. 
    
- Bearbeiten Sie die Zuweisung für bedingten Zugriff des Benutzers.
    
1. Im Azure-Portal gehen Sie **zu \> InTune- \> Richtlinien für bedingten Zugriff**
    
2. Auswählen einer Richtlinie aus der Liste
    
3. Klicken Sie auf **Benutzer und Gruppen** .
    
4. Um eine bestimmte Richtlinie auf eine Person abzuzielen, fügen Sie Sie der Liste **einschließen** hinzu. Um sicherzustellen, dass eine Person aus der Richtlinie weggelassen wird, fügen Sie Sie der **Ausschluss** Liste hinzu. 
    
Weitere Informationen: [Vorgehensweise zum Überwachen von bedingten Zugriffs Geräten](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

