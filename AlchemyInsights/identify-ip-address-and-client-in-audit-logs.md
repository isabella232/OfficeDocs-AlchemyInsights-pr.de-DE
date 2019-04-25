---
title: Identifizieren von IP-Adressen und Clients in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 7e30a638de5926aa11b8ae637613a48076d7bdc9
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32416960"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifizieren von IP-Adressen und Clients in Überwachungsprotokollen

Die IP-Adresse, die einer Aktivität eines Benutzers oder Administrators entspricht, wird in den Überwachungsprotokollen angezeigt. Die Clientinformationen werden ebenfalls protokolliert. Hier sind die Schritte zur Identifizierung solcher Informationen

1. Melden Sie sich beim [Office 365 Security _AMP_ Compliance Center](https://protection.office.com/) an.

2. Klicken Sie auf **Suchen und Untersuchung** , und wählen Sie **Überwachungsprotokoll Suche**aus.

   Wenn Sie an einer bestimmten Aktivität interessiert sind, wählen Sie Sie aus der Liste **Aktivitäten** aus. Ist dies nicht der Fall, werden alle Aktivitäten für den ausgewählten Benutzer zurückgegeben (Standardeinstellung).

   **Hinweis**: bestimmte Aktivitäten sind möglicherweise nicht im Menü " **Aktivitäten** " verfügbar; Diese Überwachungselemente werden jedoch zurückgegeben, wenn die Option **Ergebnisse für alle Aktivitäten anzeigen** ausgewählt ist (Standardeinstellung).

3. Geben Sie den Benutzernamen im Feld **Benutzer** an, wählen Sie den entsprechenden Datumsbereich für die Aktivität aus, und klicken Sie dann auf **Suchen**.

In den Ergebnissen wird die IP-Adresse für diese Aktivität im Ergebnisbereich angezeigt. Wählen Sie den Überwachungsdatensatz aus, um detaillierte Informationen im **Detail** Flyout anzuzeigen (beispielsweise Client, Benutzer, der die Aktion ausgeführt hat, usw.).

Weitere Informationen finden Sie unter [Suchen der IP-Adresse des Computers, der für den Zugriff auf ein kompromittiertes Konto verwendet wird](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
