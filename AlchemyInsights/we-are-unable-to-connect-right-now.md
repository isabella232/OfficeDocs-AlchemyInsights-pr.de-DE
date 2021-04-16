---
title: 'Aktivierungsproblem : Wir können derzeit keine Verbindung herstellen'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806441"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Beheben der Microsoft 365-Apps "Wir können jetzt keine Verbindung herstellen"

Wenn Sie diese Nachricht erhalten, versuchen Sie Folgendes:

1. Überprüfen Sie Ihre Firewall-, Antivirensoftware- und Proxyeinstellungen, um zu überprüfen, ob sie den Internetzugriff auf Microsoft 365-Apps nicht blockieren. Weitere [Informationen finden Sie unter Microsoft URLs und IP-Adressbereiche](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Wechseln Sie **zu Start**  >  **Ausführen**, und geben Sie **dann services.msc ein.** Stellen Sie sicher, dass die folgenden Dienste ausgeführt werden:
    - Automatisches Einrichten von netzwerkgebundenen Geräten
    - Netzwerklistendienst
    - Netzwerkstandortbewusstsein
    - Windows-Ereignisprotokoll

Wenn einer dieser Dienste nicht ausgeführt wird, versuchen Sie, ihn zu starten. Wenn beim Starten des Diensts ein Problem besteht, führen Sie den folgenden Befehl aus, indem Sie eine Eingabeaufforderung mit erhöhten Berechtigungen öffnen:

**sfc /scannow**

Starten Sie nach Abschluss dieses Befehls den Computer neu.

Ausführliche Informationen finden Sie unter "Leider können [wir keine Verbindung mit Ihrem Konto herstellen. Versuchen Sie es später erneut"-Fehler, wenn Sie Office von Microsoft 365 aktivieren.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)