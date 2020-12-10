---
title: 'Problembehandlung bei Voicemail '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608005"
---
# <a name="troubleshooting-voicemail"></a>Problembehandlung bei Voicemail

Stellen Sie sicher, dass das Feature busy on Busy beabsichtigt ist.

Wenn dieses Feature für diesen Benutzer nicht erforderlich ist:

1. Wechseln Sie zu [Teams Admin Center](https://admin.teams.microsoft.com/policies/calling).
1. Navigieren Sie auf der linken Seite in Richtlinien für **VoIP**  >  -**Anrufe**  >  **Verwalten von Richtlinien** für die **Anrufrichtlinie**.
1. Wählen Sie **Benutzer verwalten** aus.
1. Suchen Sie nach dem Benutzer, und ändern Sie die Anrufrichtlinie in eine, die **beschäftigt in beschäftigt ist, ist verfügbar, wenn in einem Aufruf** **von Off**.
1. Klicken Sie auf **Anwenden**.
> [!NOTE]
> Änderungen an Richtlinien können bis zu 24 Stunden dauern, bis Sie repliziert werden.

Weitere Informationen zu diesem Feature finden Sie unter: [busy on Busy steht während eines Anrufs zur Verfügung](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).
