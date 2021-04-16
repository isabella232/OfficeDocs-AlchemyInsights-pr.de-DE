---
title: Fehler "Teams 4c7"
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786668"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7-Fehler in Microsoft Teams

Dieser Fehler tritt auf, weil Microsoft Teams die Formularauthentifizierung erfordert. Wenn Sie Active Directory Federation Services (AD FS) bereitstellen, ist die Formularauthentifizierung für das Intranet standardmäßig nicht aktiviert. Wenn bei der integrierten Windows-Authentifizierung ein Fehler auftritt, werden Sie aufgefordert, sich mithilfe der Formularauthentifizierung zu anmelden.

Aktivieren Sie die Formularauthentifizierung mithilfe des AD FS Microsoft Management Console (MMC)-Snap-Ins auf dem Computer mit der lokalen Kopie von Active Directory, um dieses Problem zu beheben. Gehen Sie dazu wie folgt vor: 

1. Navigieren Sie im Navigationsbereich zu **Authentifizierungsrichtlinien**.
2. Wählen **Sie unter Aktionen** im Detailbereich die Option Globale primäre **Authentifizierung bearbeiten aus.**
3. Wählen Sie **auf der Registerkarte Intranet** die Option **Formularauthentifizierung aus.**
4. Wählen **Sie OK** (oder **Anwenden) aus.**