---
title: Begriffe, die in SharePoint Online Term Store fehlen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750450"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Aktivieren der BitLocker-Verschlüsselung mit InTune

Die Intune-Endpunktschutz Richtlinie kann zum Konfigurieren von Boitlocker-Verschlüsselungseinstellungen für Windows-Geräte verwendet werden, wie unter: Windows10 (und höher) Einstellungen zum Schützen von Geräten mithilfe von InTune beschrieben.

Beachten Sie, dass viele neuere Geräte mit Windows 10 die automatische BitLocker-Verschlüsselung unterstützen, die ohne Anwendung der MDM-Richtlinie ausgelöst wird. Dies kann sich auf die Anwendung von Richtlinien auswirken, wenn nicht Standardeinstellungen konfiguriert sind. Weitere Informationen finden Sie unter FAQ.


FAQ   f: welche Editionen von Windows unterstützen die Geräteverschlüsselung mithilfe der Endpunktschutz Richtlinie?
 A.: die Einstellungen in der InTune-Endpunktschutz Richtlinie werden mithilfe des BitLocker-CSP implementiert.Nicht alle Editionen oder Builds von Windows unterstützen den BitLocker-CSP. 
      Zu diesem Zeitpunkt Windows-Editionen: Enterprise; Education, Mobile, Mobile Enterprise und Professional (ab Build 1809) werden unterstützt.




F.: Wenn ein Gerät bereits mit BitLocker mit den Standardeinstellungen für Verschlüsselungsmethode und Verschlüsselungsstärke (XTS-AES-128) verschlüsselt ist, wird eine Richtlinie mit unterschiedlichen Einstellungen automatisch mit der erneuten Verschlüsselung des Laufwerks mit den neuen Einstellungen ausgelöst?

A: Nein. Damit die neuen Verschlüsselungseinstellungen angewendet werden, muss das Laufwerk zunächst entschlüsselt werden.

Hinweis für Geräte, die mit Autopilot registriert werden die automatische Verschlüsselung, die während der OOBE erfolgen würde, wird erst ausgelöst, wenn die Intune-Richtlinie ausgewertet wird, sodass die richtlinienbasierten Einstellungen anstelle der Standardwerte für das Betriebssystem verwendet werden können.




F. Wenn ein Gerät aufgrund der Anwendung der InTune-Richtlinie verschlüsselt wird, wird es entschlüsselt, wenn diese Richtlinie entfernt wird?

A: das Entfernen von Verschlüsselungs bezogenen Richtlinien führt nicht zur Entschlüsselung der konfigurierten Laufwerke.




F: Warum zeigt die Intune-Konformitätsrichtlinie an, dass auf meinem Gerät "BitLocker Enabled" nicht vorhanden ist, aber es ist?

A.: die Einstellung "BitLocker Enabled" in der InTune-Konformitätsrichtlinie verwendet den Windows-Client für Geräte Integritäts Bescheinigung (DHA). Dieser Client misst nur den Gerätestatus zum Zeitpunkt des Bootens. Wenn also ein Gerät seit der BitLocker-Verschlüsselung nicht neu gestartet wird, meldet der DHA-Client Dienst BitLocker nicht als aktiv.