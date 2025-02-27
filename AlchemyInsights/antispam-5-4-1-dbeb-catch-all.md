---
title: AntiSpam 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932276"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Beheben von Zustellungsproblemen bei Fehlercode 550 5.4.1 Relay-Zugriff verweigert

Dieses Problem tritt auf, wenn [überprüft wird, ob eine E-Mail-Adresse gültig ist, um Bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) beim Betreten des Microsoft-Netzwerks zu verhindern. Versuchen Sie, das Problem durch folgende Maßnahme zu beheben:

1. Ermitteln Sie, ob das Problem für eine gesamte Domäne oder eine einzelne E-Mail-Adresse spezifisch ist:
    - Gesamte Domäne: Manchmal muss die Domäne synchronisiert werden; Versuchen [Sie, die Domäne auf "Intern" und dann wieder auf "Autoritativ" festzulegen.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - Einzelne E-Mail-Adresse: Manchmal muss die Adresse synchronisiert werden; Das Ändern der SMTP-Proxyadresse und das anschließende Zurückwechseln kann hilfreich sein.
2. Bestimmen Sie, ob das Problem für eine Gruppe oder einen öffentlichen Ordner spezifisch ist. Bei einigen Objekttypen müssen die Objekte möglicherweise manuell in Azure Active Directory erstellt werden.

Wenn Sie zusätzliche Hilfe benötigen, öffnen Sie ein Supportticket, und geben Sie den Umfang des Problems an (einschließlich des Typs des Objekts, an das Sie senden), damit wir Sie besser unterstützen können.