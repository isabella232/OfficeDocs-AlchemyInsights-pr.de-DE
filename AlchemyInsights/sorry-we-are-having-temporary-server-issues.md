---
title: Beheben von Microsoft 365-apps Sorry, wir haben eine temporäre Server Problemmeldung
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582702"
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