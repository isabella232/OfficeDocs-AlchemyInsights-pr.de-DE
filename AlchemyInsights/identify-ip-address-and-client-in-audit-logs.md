---
title: Identifizieren der IP-Adresse und des Clients in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716387"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifizieren der IP-Adresse und des Clients in Überwachungsprotokollen

Die IP-Adresse, die einer Aktivität eines Microsoft 365-Benutzers oder-Administrators entspricht, wird in den Überwachungsprotokollen angezeigt. Die Clientinformationen werden ebenfalls protokolliert. Hier sind die Schritte zum Identifizieren solcher Informationen.

1. Melden Sie sich beim [Microsoft 365 Security & Compliance Center](https://protection.office.com/)an.

2. Wechseln Sie zur **Search** > Suchseite**Überwachungsprotokoll** suchen.

   Wenn Sie an einer bestimmten Aktivität interessiert sind, wählen Sie diese in der Liste **Aktivitäten** aus. Wenn dies nicht der Fall ist, werden alle Aktivitäten für den ausgewählten Benutzer zurückgegeben (Standardeinstellung).

   **Hinweis**: bestimmte Aktivitäten stehen im Menü **Aktivitäten** möglicherweise nicht zur Verfügung; Diese Überwachungselemente werden jedoch zurückgegeben, wenn **Ergebnisse für alle Aktivitäten anzeigen** ausgewählt ist (Standardeinstellung).

3. Geben Sie im Feld **Benutzer** den Benutzernamen an, wählen Sie den entsprechenden Datumsbereich für die Aktivität aus, und klicken Sie dann auf **Suchen**.

In den Ergebnissen können Sie die IP-Adresse für diese Aktivität im Ergebnisbereich anzeigen. Wählen Sie den Überwachungseintrag aus, um detaillierte Informationen im Flyout **Details** anzuzeigen (beispielsweise Client, Benutzer, der eine Aktion ausgeführt hat, usw.).

Weitere Informationen finden Sie unter [Suchen der IP-Adresse des Computers, der für den Zugriff auf ein kompromittiertes Konto verwendet](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)wurde.
