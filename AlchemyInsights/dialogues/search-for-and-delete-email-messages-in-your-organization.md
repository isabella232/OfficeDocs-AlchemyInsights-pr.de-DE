---
title: Suchen nach und Löschen von E-Mail-Nachrichten in der Organisation
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500966"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Suchen nach und Löschen von E-Mail-Nachrichten in der Organisation

Führen Sie die folgenden Schritte aus:

1. Wenn Sie kein globaler Administrator sind, muss Ihr Konto zur Rollengruppe **eDiscovery-Manager** oder zur Verwaltungsrolle **"Compliancesuche"** hinzugefügt werden, um nach Nachrichten zu suchen. Zum Löschen von Nachrichten müssen Sie  der Rollengruppe Organisationsverwaltung oder der Verwaltungsrolle Suchen und Löschen **beitreten.** Berechtigungen für diese Rollen werden im [Security & Compliance Center zugewiesen.](https://protection.office.com)
2. [Erstellen Sie eine Inhaltssuche,](https://docs.microsoft.com/office365/securitycompliance/content-search) um die zu löschende Nachricht zu finden.
3. [Stellen Sie eine Verbindung mit der Security & Compliance Center PowerShell her](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Wenn Sie MFA verwenden, lesen Sie die folgenden Anweisungen: Verbinden mit Security [& Compliance Center PowerShell mithilfe der mehrstufigen Authentifizierung](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Nachricht löschen: Führen Sie das `New-ComplianceSearchAction` Cmdlet aus, um die Nachricht zu löschen. Gelöschte Nachrichten werden in den Ordner "Wiederherstellbare Elemente" eines Benutzers verschoben. Ein Beispielbefehl finden Sie unter [Schritt 3: Löschen der Nachricht.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
