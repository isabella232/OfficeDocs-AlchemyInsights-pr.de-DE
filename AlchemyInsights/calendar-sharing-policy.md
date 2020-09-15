---
title: 618 Kalenderfreigabe Richtlinie
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684229"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Richtlinienfehler beim Freigeben eines Kalenders

1. Führen Sie entsprechend ihrer Situation eine der folgenden Aktionen aus:
    - Stellen Sie mithilfe von Remote-PowerShell eine Verbindung zu Exchange Online her. Weitere Informationen finden Sie unter [Herstellen einer Verbindung mit Exchange Online mithilfe von Remote-PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Öffnen Sie auf dem lokalen Server das Exchange-Verwaltungsshell.
2. Bestimmen Sie die Freigaberichtlinie, die dem Benutzer zugewiesen ist. Führen Sie dazu den folgenden Befehl aus, und beachten Sie die zurückgegebene Richtlinie:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Aktualisieren Sie die Freigaberichtlinie für den Benutzer. Gehen Sie dazu wie folgt vor:
    - Öffnen Sie das Exchange Admin Center.
    - Klicken Sie auf **Organisation**, und doppelklicken Sie dann auf die Richtlinie, die dem Benutzer unter **individuelle Freigabe**zugewiesen ist. Dies ist die Richtlinie, die in Schritt 2 zurückgegeben wurde.
    - Wählen Sie auf der Seite Freigabe Regel die Kalenderfreigabe Ebene aus, die Sie zulassen möchten unter Geben Sie an, **welche Informationen Sie freigeben**möchten. Klicken Sie auf **Speichern**.

Weitere Informationen finden Sie unter: ["die Richtlinie erlaubt nicht das Erteilen von Berechtigungen auf dieser Ebene für einen oder mehrere Empfänger Fehler, wenn der Benutzer versucht, Kalender freizugeben](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
