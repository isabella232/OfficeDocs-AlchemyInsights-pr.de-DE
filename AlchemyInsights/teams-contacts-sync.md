---
title: Teams-Kontaktsynchronisierung
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004610"
- "11540"
ms.openlocfilehash: 0ffa91f0e31a4904db87f0df6d9b4c51b05ae2758a5ce0d96c77ef4456f6d033
ms.sourcegitcommit: 71501cde5bcb73f4dcf23944d400a4db10f37033
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/09/2021
ms.locfileid: "57807192"
---
# <a name="teams-contacts-sync"></a>Teams-Kontaktsynchronisierung

Teams verwendet Kontakte im Active Directory Ihrer Organisation sowie Kontakte, die dem Outlook-Standardordner des Benutzers hinzugefügt wurden. Wenn Kontakte nicht in Microsoft Teams angezeigt werden, versuchen Sie Folgendes:

**Hinweis:** Wenn die Informationen für einen oder mehrere Kontakte kürzlich aktualisiert wurden, kann es bis zu 48 Stunden dauern, bis die Kontakte synchronisiert sind.

1. Melden Sie sich bei Teams ab und starten Sie es neu. Überprüfen Sie, ob Ihre Kontakte angezeigt werden.
1. Löschen Sie den Teams-Cache:
    1. Browsen Sie zu **%appdata%\Microsoft\Teams**.
    1. Löschen Sie den Inhalt des Ordners.
    1. Starten Sie den Computer neu und versuchen Sie, Teams zu starten.
1. Wenn sich der Kontakt in Outlook befindet, stellen Sie sicher, dass er der Kontaktliste hinzugefügt wird. Wählen Sie in Outlook in der Adressleiste **Datei** aus, und wählen Sie dann **Zu Kontakten hinzufügen** aus.
1. Stellen Sie sicher, dass das Exchange-Postfach online gehostet ist (nicht lokal). Weitere Informationen finden Sie unter [Interaktion von Exchange und Microsoft Teams](/microsoftteams/exchange-teams-interact).
1. Stellen Sie sicher, dass die Telefonnummer des Kontaktes zu den Kontaktinformationen hinzugefügt ist.
1. Suchen Sie in der Suchleiste nach der E-Mail des Kontakts. Kontakte, die Sie mit der Kontaktliste synchronisieren können.
