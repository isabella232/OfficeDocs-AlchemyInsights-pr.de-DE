---
title: Erstellen einer e-Mail catch all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286109"
---
# <a name="create-an-email-catch-all"></a>Erstellen einer e-Mail catch all

Für die Verwendung eines catch all wird dringend abgeraten. Es ist besser, einen Bounce-Back an den Absender zu übermitteln, wenn Absender wissen, dass Ihre Nachricht nicht als adressiert zugestellt werden konnte, damit Sie Aktionen ausführen können. Sie können das überwachte Postfach auch so einschränken, dass nur frühere gültige e-Mail-Adressen erfasst werden. 

Alle Catch-Postfächer werden viel Spam erhalten und können eventuell gefüllt werden, wenn Sie nicht genau überwacht werden. (Es gibt Empfangs Grenzwerte.) 

Wenn Sie den Vorgang fortsetzen möchten, führen Sie die folgenden Schritte aus:

1. Erstellen Sie eine dynamische Verteilergruppe & "alle Empfängertypen einschließen".

2. Erstellen Sie ein dediziertes Postfach zum Abfangen von e-Mails, beispielsweise CatchAll@Domain.com.

3. Legen Sie für die spezifische Domäne den DomainType auf "InternalRelay" fest. Wenn Sie später den catch all entfernen, müssen Sie die Domäne wieder auf autorisierend festlegen.

4. Erstellen Sie wie folgt eine Mailflow-Transport Regel:

    - Wenn der Absender "außerhalb der Organisation" ist
    - Umleiten der Nachricht an CatchAll@Domain.com
    - Außer wenn der Empfänger Mitglied von ALLUSERS@Domain.com ist (Verteilergruppe enthält alle Mitglieder)
    - Sicherstellen, dass überprüft wird, ob neue Postfächer der dynamischen Verteilergruppe hinzugefügt werden
