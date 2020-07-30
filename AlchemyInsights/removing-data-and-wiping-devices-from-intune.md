---
title: Entfernen von Daten und Zurücksetzen des Geräts aus Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434605"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Entfernen von Daten und Zurücksetzen des Geräts aus Intune

Die Aktionen "Gerät zurücksetzen" und "Gerät abkoppeln" können verwendet werden, um von Intune verwaltete Unternehmensdaten zu entfernen oder eine Zurücksetzung auf Werkseinstellungen durchzuführen und das Gerät auf seine Standardeinstellungen zurückzusetzen.

1. Melden Sie sich bei der Microsoft 365-Geräteverwaltung an, und navigieren Sie zu **Geräte** > **Alle Geräte**.
2. Wählen Sie das Gerät aus, das Sie zurücksetzen möchten.
3. Wählen Sie die Art der Remotezurücksetzung aus, die Sie durchführen möchten. Durch das Abkoppeln werden nur organisatorische Informationen gelöscht, während eine vollständige Zurücksetzung das Gerät auf die Werkseinstellungen zurücksetzt.
4. Wählen Sie zum Bestätigen **Ja** aus. Bis die Zurücksetzung abgeschlossen ist, wird als Status der Geräteaktion "Abkoppeln ausstehend" angezeigt.</br>
    Nachdem der Vorgang abgeschlossen ist, wird das mobile Gerät nicht mehr in der Liste der verwalteten Geräte angezeigt.

**Hinweis** Unternehmensdaten können nicht von Geräten entfernt werden, die mit Azure AD VERBUNDEN sind.

Vollständige Informationen zu den Auswirkungen der Aktionen "Abkoppeln" und "Zurücksetzen", beispielsweise, was aufbewahrt und was gelöscht wird, finden Sie unter [Entfernen von Geräten durch Zurücksetzen, Abkoppeln oder manuelles Aufheben der Registrierung des Geräts](https://docs.microsoft.com/intune/devices-wipe).

Informationen dazu, wie Sie alle Daten von einem macOS-Gerät löschen, finden Sie unter [Löschen aller Daten von einem macOS-Gerät](https://docs.microsoft.com/intune/device-erase).