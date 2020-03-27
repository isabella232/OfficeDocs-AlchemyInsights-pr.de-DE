---
title: Kalendersymbol wird im Teams-Client nicht angezeigt
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931978"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Kalendersymbol wird im Teams-Client nicht angezeigt

Die Registerkarte „Kalender“ in Teams muss über Exchange-Webdienste auf ein Exchange-Postfach zugreifen können. Das Exchange-Postfach kann online oder lokal sein. Vergewissern Sie sich für Onlinebenutzer, für die die Registerkarte „Kalender“ nicht angezeigt wird, dass [ sie für ein Exchange Online-Postfach lizenziert sind und das Postfach aktiviert](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes) ist.

Wenn der Benutzer über ein gültiges Postfach in Exchange Online verfügt, die Registerkarte „Kalender“ aber immer noch nicht angezeigt wird, tritt möglicherweise ein Netzwerkproblem auf. Verwenden Sie die [Microsoft-Remoteverbindungsuntersuchung](https://testconnectivity.microsoft.com/), und führen Sie die **Verbindungstests für Microsoft Exchange-Webdienste** für den betroffenen Benutzer durch.

Überprüfen Sie schließlich die [Teams-Apps –-App-Setup-Richtlinien](https://admin.teams.microsoft.com/policies/app-setup), um sicherzustellen, dass die Kalender-App nicht aus der auf den Benutzer angewendeten Richtlinie entfernt wurde (höchstwahrscheinlich die globale Richtlinie (organisationsweiter Standard)****.

Wenn Ihre Benutzer lokal sind, müssen Sie sicherstellen, dass Ihre Hybridkonfiguration fehlerfrei ist. Verwenden Sie den [Assistenten für die Hybridkonfiguration](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) zur Problembehandlung.

Beachten Sie, dass für [Teams Exchange 2016 CU3 oder höher erforderlich ist](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
