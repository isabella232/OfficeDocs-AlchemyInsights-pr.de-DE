---
title: Überwachen des bedingten Zugriffs auf Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/03/2021
ms.locfileid: "50417321"
---
# <a name="monitor-intune-conditional-access"></a>Überwachen des bedingten Zugriffs auf Intune

Benutzer mit bedingten Zugriff erhalten eine Benachrichtigungs-E-Mail, wenn sie die Zugriffsanforderungen Ihrer Organisation nicht erfüllen. Zur Lösung empfehlen wir eine oder mehrere der folgenden Lösungen:

1. Wenn angenommen wird, dass das Gerät registriert ist, empfehlen Sie dem Benutzer, zur Unternehmensportal-App zu wechseln und zu überprüfen, ob es im Unternehmensportal angezeigt wird. Andern falls nicht, muss der Benutzer das Gerät registrieren.
1. Wechseln Sie im Azure-Portal zu **Intune**  >  **Device compliance**. 
1. Klicken Sie unter **Überwachen** auf Gerätekonformität, um den Bericht zur Gerätekonformität anzeigen zu können, um zu überprüfen, ob das Gerät des Benutzers als kompatibel **gekennzeichnet ist.**
1. Wechseln Sie im Azure-Portal zu **Intune**  >  **Device compliance**. Klicken **Sie unter Verwalten** auf **Richtlinien**. Überprüfen Sie in der Liste der Compliancerichtlinien, ob dem Gerät Ihres Benutzers ein Profil zugewiesen ist. Wenn kein Profil zugewiesen ist, kann Intune den Kompatibilitätsstatus des Geräts nicht bestätigen.
1. Bearbeiten Sie die Zuweisung für bedingten Zugriff des Benutzers.
1. Navigieren Sie im Azure-Portal zu   >  **Intune-Richtlinien** für bedingten  >   **Zugriff,** wählen Sie in der Liste eine Richtlinie aus, und klicken Sie auf Benutzer und Gruppen .
1. Um eine bestimmte Richtlinie auf eine Person zu zielen, fügen Sie sie der **Include-Liste hinzu.** Um sicherzustellen, dass eine Person aus der Richtlinie ausgelassen wird, fügen Sie sie der **Liste Ausschließen hinzu.**

**Hilfreiche Links:**

- [Übersicht über die Gerätekonformität](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Problembehandlung bei der Zertifizierungsstelle](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Problembehandlungsrichtlinie](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Überwachen der Intune-Gerätekonformität](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Diese Schritte sind nur bei der Problembehandlung für das Azure Active Directory-Feature Bedingter Zugriff hilfreich. Es ist auch möglich, ein Gerät unter Quarantäne zu stellen, das den E-Mail-Zugriff mit der Exchange-Richtlinie blockiert. Weitere Informationen zur Exchange-Geräteverwaltung finden Sie [**hier**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).
