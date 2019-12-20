---
title: Microsoft Teams-4c7-Fehler
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796120"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7-Fehler in Microsoft Teams

Dieser Fehler tritt auf, weil Microsoft Teams die Formularauthentifizierung erfordert. Wenn Sie Active Directory Verbunddienste (AD FS) bereitstellen, ist die Formularauthentifizierung standardmäßig nicht für das Intranet aktiviert. Wenn die integrierte Windows-Authentifizierung fehlschlägt, werden Sie aufgefordert, sich mit der Formularauthentifizierung anzumelden.

Um dieses Problem zu beheben, aktivieren Sie die Formularauthentifizierung mithilfe des AD FS-MMC-Snap-Ins (Microsoft Management Console) auf dem Computer mit der lokalen Kopie von Active Directory. Führen Sie hierzu die folgenden Schritte aus: 

1. Navigieren Sie im Navigationsbereich zu **Authentifizierungsrichtlinien**.
2. Wählen Sie im Detailbereich unter **Aktionen** die Option **globale primäre Authentifizierung bearbeiten**aus.
3. Wählen Sie auf der Registerkarte **Intranet** die Option **Formularauthentifizierung**aus.
4. Wählen Sie **OK** (oder **anwenden**) aus.