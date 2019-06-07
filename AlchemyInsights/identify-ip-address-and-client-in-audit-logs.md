---
title: Identifizieren der IP-Adresse und des Clients in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 87e0d414fe02d5074a56cd5a77d50db1464b7faf
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752059"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifizieren der IP-Adresse und des Clients in Überwachungsprotokollen

Die IP-Adresse, die einer Aktivität durch einen Benutzer oder Administrator entspricht, wird in den Überwachungsprotokollen angezeigt. Die Clientinformationen werden ebenfalls protokolliert. Hier sind die Schritte zum Identifizieren solcher Informationen.

1. Melden Sie sich beim [Office 365 Security #a0 Compliance Center](https://protection.office.com/) an.

2. Klicken Sie auf **Suche und Untersuchung** , und wählen Sie **Überwachungsprotokoll Suche**aus.

   Wenn Sie an einer bestimmten Aktivität interessiert sind, wählen Sie diese in der Liste **Aktivitäten** aus. Wenn dies nicht der Fall ist, werden alle Aktivitäten für den ausgewählten Benutzer zurückgegeben (Standardeinstellung).

   **Hinweis**: bestimmte Aktivitäten stehen im Menü **Aktivitäten** möglicherweise nicht zur Verfügung; Diese Überwachungselemente werden jedoch zurückgegeben, wenn **Ergebnisse für alle Aktivitäten anzeigen** ausgewählt ist (Standardeinstellung).

3. Geben Sie im Feld **Benutzer** den Benutzernamen an, wählen Sie den entsprechenden Datumsbereich für die Aktivität aus, und klicken Sie dann auf **Suchen**.

In den Ergebnissen können Sie die IP-Adresse für diese Aktivität im Ergebnisbereich anzeigen. Wählen Sie den Überwachungseintrag aus, um detaillierte Informationen im Flyout **Details** anzuzeigen (beispielsweise Client, Benutzer, der eine Aktion ausgeführt hat, usw.).

Weitere Informationen finden Sie unter [Suchen der IP-Adresse des Computers, der für den Zugriff auf ein kompromittiertes Konto verwendet](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)wurde.
