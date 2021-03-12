---
title: Überwachen des bedingten Zugriffs
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708673"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Überwachen des bedingten Zugriffs für Exchange

Benutzer mit bedingten Zugriff erhalten eine Benachrichtigungs-E-Mail, wenn sie die Zugriffsanforderungen Ihrer Organisation nicht erfüllen. Zur Lösung empfehlen wir eine oder mehrere der folgenden Lösungen:

- Wenn angenommen wird, dass das Gerät registriert ist, empfehlen Sie dem Benutzer, zur Unternehmensportal-App zu wechseln und zu überprüfen, ob es im Unternehmensportal angezeigt wird. Andern falls nicht, sollte der Benutzer das Gerät registrieren.
- Wechseln Sie im Azure-Portal zu Intune > Gerätekonformität. Klicken Sie unter Überwachen auf Gerätekonformität. Zeigen Sie den Bericht zur Gerätekonformität an, um zu überprüfen, ob das Gerät des Benutzers als kompatibel gekennzeichnet ist.
- Wechseln Sie im Azure-Portal zu Intune > Gerätekonformität. Klicken Sie unter Verwalten auf Richtlinien. Überprüfen Sie in der Liste der Compliancerichtlinien, ob dem Gerät Ihres Benutzers ein Profil zugewiesen ist. Wenn kein Profil zugewiesen ist, kann Intune den Kompatibilitätsstatus des Geräts nicht bestätigen.
- Bearbeiten Sie die Zuweisung für bedingten Zugriff des Benutzers.

1. Wechseln Sie im Azure-Portal zu  >  **Intune-Richtlinien für bedingten**  >  **Zugriff.**
2. Wählen Sie eine Richtlinie aus der Liste aus.
3. Klicken Sie auf Benutzer und Gruppen.
4. Um eine bestimmte Richtlinie auf eine Person zu zielen, fügen Sie sie der Include-Liste hinzu. Um sicherzustellen, dass eine Person aus der Richtlinie ausgelassen wird, fügen Sie sie der Liste Ausschließen hinzu.

Hilfreiche Links:

[Übersicht über die Gerätekonformität](https://docs.microsoft.com/intune/device-compliance-get-started)

[Problembehandlung bei der Zertifizierungsstelle](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Problembehandlungsrichtlinie](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Überwachen der Intune-Gerätekonformität](https://docs.microsoft.com/intune/compliance-policy-monitor)

Hinweis: Diese Schritte sind nur bei der Problembehandlung für das Azure Active Directory-Feature Bedingter Zugriff hilfreich. Es ist auch möglich, ein Gerät unter Quarantäne zu stellen, das den E-Mail-Zugriff mit der Exchange-Richtlinie blockiert. Weitere Informationen zur Exchange-Geräteverwaltung finden Sie [hier]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
