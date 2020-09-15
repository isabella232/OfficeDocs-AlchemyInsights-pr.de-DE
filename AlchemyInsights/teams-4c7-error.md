---
title: Microsoft Teams-4c7-Fehler
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700202"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7-Fehler in Microsoft Teams

Dieser Fehler tritt auf, weil Microsoft Teams die Formularauthentifizierung erfordert. Wenn Sie Active Directory Verbunddienste (AD FS) bereitstellen, ist die Formularauthentifizierung standardmäßig nicht für das Intranet aktiviert. Wenn die integrierte Windows-Authentifizierung fehlschlägt, werden Sie aufgefordert, sich mit der Formularauthentifizierung anzumelden.

Um dieses Problem zu beheben, aktivieren Sie die Formularauthentifizierung mithilfe des AD FS-MMC-Snap-Ins (Microsoft Management Console) auf dem Computer mit der lokalen Kopie von Active Directory. Gehen Sie dazu wie folgt vor: 

1. Navigieren Sie im Navigationsbereich zu **Authentifizierungsrichtlinien**.
2. Wählen Sie im Detailbereich unter **Aktionen** die Option **globale primäre Authentifizierung bearbeiten**aus.
3. Wählen Sie auf der Registerkarte **Intranet** die Option **Formularauthentifizierung**aus.
4. Wählen Sie **OK** (oder **anwenden**) aus.