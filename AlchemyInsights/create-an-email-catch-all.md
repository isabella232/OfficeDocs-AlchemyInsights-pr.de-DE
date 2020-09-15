---
title: Erstellen einer e-Mail catch all
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
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712985"
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
