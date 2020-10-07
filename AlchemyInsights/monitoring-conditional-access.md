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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366427"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Überwachen des bedingten Zugriffs für Exchange

Benutzer, die auf bedingten Zugriff abzielen, erhalten eine Benachrichtigungs-e-Mail, wenn Sie die Zugriffsanforderungen Ihrer Organisation nicht erfüllen. Zur Behebung empfehlen wir eine oder mehrere der folgenden Lösungen:

- Wenn Sie davon ausgehen, dass das Gerät registriert ist, empfehlen Sie dem Benutzer, zur Unternehmensportal-APP zu wechseln und zu überprüfen, ob er im Unternehmensportal angezeigt wird. Wenn dies nicht der Fall ist, sollte der Benutzer das Gerät registrieren.
- Wechseln Sie im Azure-Portal zu InTune-> Gerätekompatibilität. Klicken Sie unter Überwachung auf Gerätekompatibilität. Zeigen Sie Ihren Geräte Kompatibilitätsbericht an, um zu überprüfen, ob das Gerät des Benutzers als konform gekennzeichnet ist.
- Wechseln Sie im Azure-Portal zu InTune-> Gerätekompatibilität. Klicken Sie unter Verwalten auf Richtlinien. Überprüfen Sie in der Liste der Konformitätsrichtlinien, ob ein Profil dem Gerät Ihres Benutzers zugewiesen ist. Wenn kein Profil zugewiesen ist, kann InTune den Kompatibilitätsstatus des Geräts nicht bestätigen.
- Bearbeiten Sie die Zuweisung für bedingten Zugriff des Benutzers.

1. Navigieren Sie im Azure-Portal zu **InTune**  >  **Conditional access**  >  -**Richtlinien**für bedingten Zugriff.
2. Wählen Sie eine Richtlinie aus der Liste aus.
3. Klicken Sie auf Benutzer und Gruppen.
4. Um eine bestimmte Richtlinie auf eine Person abzuzielen, fügen Sie Sie der Liste einschließen hinzu. Um sicherzustellen, dass eine Person aus der Richtlinie weggelassen wird, fügen Sie Sie der Ausschlussliste hinzu.

Hilfreiche Links:

[Übersicht über die Gerätekompatibilität](https://docs.microsoft.com/intune/device-compliance-get-started)

[Problembehandlung bei ca](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Problem behandlungsrichtlinie](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[Überwachen der InTune-Gerätekompatibilität](https://docs.microsoft.com/intune/compliance-policy-monitor)

Hinweis: diese Schritte sind nur hilfreich bei der Problembehandlung für den bedingten Zugriff auf Azure Active Directory Feature. Es ist auch möglich, ein Gerät zu isolieren, das den e-Mail-Zugriff mit der Exchange-Richtlinie blockiert. Weitere Informationen zur Exchange-Geräteverwaltung finden Sie [hier](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).
