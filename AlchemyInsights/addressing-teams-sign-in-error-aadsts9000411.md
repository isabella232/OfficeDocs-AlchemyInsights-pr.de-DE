---
title: Ansprechen von Teams-Anmeldefehler AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/20/2020
ms.locfileid: "44328798"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Ansprechen von Teams-Anmeldefehler AADSTS9000411

Wenn Sie sich bei Microsoft Teams anmelden, kann die Fehlermeldung angezeigt werden: **Es tut uns leid, aber wir haben Probleme, Sie in AADSTS9000411 anzumelden: Die Anforderung ist nicht richtig formatiert. Der Parameter "login_hint" ist doppelt vorhanden.**

Um dieses Problem zu beheben, stellen Sie bitte sicher, dass Ihre Microsoft Teams-Clients aktualisiert sind. Weitere Informationen zur Aktualisierung Ihres Clients finden Sie unter [Microsoft Teams aktualisieren](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Wenn Sie Ihren Client aus irgendeinem Grund nicht aktualisieren können, werden durch das Abmelden des Clients die meisten zwischengespeicherten Daten gelöscht. Wenn Sie jedoch nach der Abmeldung/Anmeldung immer noch Probleme haben, beenden Sie Teams und löschen Sie bitte Ihren Clientcache, indem Sie die folgenden Schritte ausführen:
1. Microsoft Teams schließen.
2. Wechseln Sie zu: %appdata%\microsoft\teams, und löschen Sie alle Dateien.
3. Microsoft Teams erneut öffnen.
