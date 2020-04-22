---
title: Aktivierungsproblem – jetzt können wir keine Verbindung herstellen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716171"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Beheben der Office-Apps "Wir können jetzt keine Verbindung herstellen"-Nachricht

Wenn Sie diese Meldung erhalten, versuchen Sie Folgendes:

1. Überprüfen Sie Ihre Firewall, Antivirensoftware und Proxyeinstellungen, um sicherzustellen, dass der Internet Zugriff auf Office-Apps nicht blockiert wird. Siehe [Microsoft-URLs und IP-Adressbereiche](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Wechseln Sie zu **Start** > **Ausführen**, und geben Sie **Services. msc**ein. Stellen Sie sicher, dass die folgenden Dienste installiert sind:
    - Mit dem Netzwerk verbundene Geräte werden automatisch eingerichtet
    - Netzwerklisten Dienst
    - Netzwerkstandort Erkennung
    - Windows-Ereignisprotokoll

Wenn einer dieser Dienste nicht aktiv ist, versuchen Sie, ihn zu starten. Wenn beim Starten des Diensts ein Problem auftritt, führen Sie den folgenden Befehl aus, indem Sie eine Eingabeaufforderung mit erhöhten Berechtigungen öffnen:

**sfc-/scannow**

Nachdem dieser Befehl abgeschlossen ist, starten Sie den Computer neu.

Ausführliche Informationen finden Sie unter ["Sorry, wir können keine Verbindung zu Ihrem Konto herstellen. Versuchen Sie es später erneut "Fehler beim Aktivieren von Office von Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).