---
title: Beheben von Office-Apps Sorry, wir haben eine temporäre Server Problemmeldung
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
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627989"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Beheben der Office-Apps "Sorry, wir haben temporäre Server Probleme"-Nachricht

Wenn Sie diese Meldung erhalten, versuchen Sie Folgendes:

1. Überprüfen Sie Ihre Firewall, Antivirensoftware und Proxyeinstellungen, um sicherzustellen, dass der Internet Zugriff auf Office-Apps nicht blockiert wird. Siehe [Office 365 URLs und IP-Adressbereiche](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Wechseln Sie zu **Start** > **Ausführen**, und geben Sie **Services. msc**ein. Stellen Sie sicher, dass die folgenden Dienste installiert sind:
    - Mit dem Netzwerk verbundene Geräte werden automatisch eingerichtet
    - Netzwerklisten Dienst
    - Netzwerkstandort Erkennung
    - Windows-Ereignisprotokoll

Wenn einer dieser Dienste nicht aktiv ist, versuchen Sie, ihn zu starten. Wenn beim Starten des Diensts ein Problem auftritt, führen Sie den folgenden Befehl aus, indem Sie eine Eingabeaufforderung mit erhöhten Berechtigungen öffnen:

**sfc-/scannow**

Nachdem dieser Befehl abgeschlossen ist, starten Sie den Computer neu.

Ausführliche Informationen finden Sie unter ["Sorry, wir können keine Verbindung zu Ihrem Konto herstellen. Versuchen Sie es später erneut "Fehler beim Aktivieren von Office aus Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).