---
title: Beheben von Microsoft 365-apps Sorry, wir haben eine temporäre Server Problemmeldung
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758244"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Beheben der Microsoft 365-Apps "Sorry, wir haben temporäre Server Probleme"-Nachricht

Wenn Sie diese Meldung erhalten, versuchen Sie Folgendes:

1. Überprüfen Sie Ihre Firewall, Antivirensoftware und Proxyeinstellungen, um sicherzustellen, dass der Internet Zugriff auf Microsoft 365-apps nicht blockiert wird. Siehe [URLs und IP-Adressbereiche](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Wechseln Sie zu **Start**  >  **Ausführen**, und geben Sie **Services. msc**ein. Stellen Sie sicher, dass die folgenden Dienste installiert sind:
    - Mit dem Netzwerk verbundene Geräte werden automatisch eingerichtet
    - Netzwerklisten Dienst
    - Netzwerkstandort Erkennung
    - Windows-Ereignisprotokoll

Wenn einer dieser Dienste nicht aktiv ist, versuchen Sie, ihn zu starten. Wenn beim Starten des Diensts ein Problem auftritt, führen Sie den folgenden Befehl aus, indem Sie eine Eingabeaufforderung mit erhöhten Berechtigungen öffnen:

**sfc-/scannow**

Nachdem dieser Befehl abgeschlossen ist, starten Sie den Computer neu.

Ausführliche Informationen finden Sie unter ["Sorry, wir können keine Verbindung zu Ihrem Konto herstellen. Versuchen Sie es später erneut "Fehler beim Aktivieren](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).