---
title: Antispam 5.4.1 Blockierung catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4a56cfe74d8940e53a316d3bcc3809e8666c2e37
ms.sourcegitcommit: a8945ab0008f138b2992175b0640e78a505d29e1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/04/2019
ms.locfileid: "37964157"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Beheben von Übermittlungsproblemen für den Fehlercode 550 5.4.1 Relay-Zugriff verweigert

Dieses Problem tritt auf [, wenn Sie überprüfen, ob eine e-Mail-Adresse gültig ist, um Abpraller](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) beim Eintritt in das Office 365 Netzwerk zu verhindern. Versuchen Sie, das Problem durch folgende Maßnahme zu beheben:

1. Ermitteln, ob das Problem für eine ganze Domäne oder eine einzelne e-Mail-Adresse spezifisch ist:
    - Gesamte Domäne: Manchmal muss die Domäne synchronisiert werden; versuchen Sie [, die Domäne auf Internal und dann auf autorisierend zurücksetzen](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
     - Einzelne e-Mail-Adresse: Manchmal muss die Adresse synchronisiert werden; Wenn Sie die SMTP-Proxyadresse ändern und dann zurück ändern, kann dies hilfreich sein.
2. Ermitteln Sie, ob das Problem für eine Gruppe oder einen öffentlichen ordnerspezifisch ist. Für einige Objekttypen müssen die Objekte möglicherweise manuell in Azure Active Directory erstellt werden.

Wenn Sie weitere Hilfe benötigen, öffnen Sie ein Support Ticket, und geben Sie den Umfang des Problems an (includidng den Typ des Objekts, an das Sie senden), damit wir Sie besser unterstützen können.