---
title: Beheben des Fehlers "Sie Anwendung wurde nicht erkannt"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 498c2ec78bc9f4a7bc7d77d12b488be2cf0bf79a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666977"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Beheben des Fehlers "Sie Anwendung wurde nicht erkannt"

Der von Intune gemeldete App-Installationsfehler "Die Anwendung wurde nicht erkannt" nach erfolgreichem Abschluss der Installation kann auf allen wichtigen Betriebssystemplattformen (Windows, IOS und Android) auftreten.

Zu den häufigsten Szenarien, die diesen Fehler generieren, gehören:

- Die App wurde nach der ersten Bereitstellung außerhalb von Intune (über den App Store eines Drittanbieters) aktualisiert. Einige Anwendungen wie Google Chrome können beispielsweise automatische Updates durchführen.
- Ein Benutzer hat die App nach der Erstinstallation deinstalliert.

Um dieses Problem zu vermeiden, untersuchen Sie zuerst die betroffenen Geräte, um das Szenario zu ermitteln, in dem der Fehler aufgetreten ist.

- Wenn die App außerhalb von Intune aktualisiert wurde, kann die App-Bereitstellung so festgelegt werden, dass diese Anwendungsversion ignoriert wird. Legen Sie dazu unter **App-Konfiguration > App-Informationen** die Option **App-Version ignorieren** auf **Ja** fest.
- Bei der Ausrichtung auf den Kunden kann es sinnvoll sein, die Anwendung als "Erforderlich" bereitzustellen, um sicherzustellen, dass die neueste Version bereitgestellt wird.
- Alternativ können Sie auf der iOS-Plattform die mit dem Apple-Volumenlizenzprogramm verknüpfte **AutoUpdate**-Funktionalität verwenden, die so konfiguriert werden kann, dass automatisch eine Aktualisierung auf neue Anwendungsversionen durchgeführt wird, sobald diese verfügbar sind.

Weitere Informationen zur Behandlung von Problemen bei der Installation von Apps finden Sie unter [Problembehandlung bei der App-Installation](https://docs.microsoft.com/intune/troubleshoot-app-install).
