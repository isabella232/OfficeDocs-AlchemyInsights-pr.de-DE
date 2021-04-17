---
title: Erstellen einer E-Mail-Catch-Nachricht
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
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816199"
---
# <a name="create-an-email-catch-all"></a>Erstellen einer E-Mail-Catch-Nachricht

Die Verwendung eines catch all wird dringend abgeraten. Es ist besser, eine Unzustellbarkeit an den Absender zu senden, damit Absender wissen, dass ihre Nachricht nicht als adressiert zugestellt werden konnte, damit sie Maßnahmen ergreifen können. Sie können das überwachte Postfach auch darauf beschränken, nur zuvor gültige E-Mail-Adressen zu fangen. 

Jedes Catch-All-Postfach erhält eine menge Spam und kann schließlich füllen, wenn es nicht genau überwacht wird. (Es gibt Empfangsgrenzwerte.) 

Wenn Sie den Vorgang fortsetzen möchten, führen Sie die folgenden Schritte aus:

1. Erstellen einer dynamischen Verteilergruppe & "Alle Empfängertypen" enthalten.

2. Erstellen Sie ein dediziertes Postfach zum Abfangen von E-Mails, z. B. catchall@domain.com.

3. Legen Sie für die spezifische Domäne domainType auf "InternalRelay" festgelegt. Wenn Sie später die catch all entfernen, stellen Sie sicher, dass die Domäne wieder auf Autoritative festgelegt wird.

4. Erstellen Sie eine Mailflow-Transportregel wie folgt:

    - Wenn der Absender "Außerhalb der Organisation" ist
    - Umleiten der Nachricht an Catchall@domain.com
    - Es sei denn, der Empfänger ist Mitglied allusers@domain.com (Verteilergruppe enthält alle Mitglieder)
    - Sicherstellen, dass der dynamischen Verteilergruppe neue Postfächer hinzugefügt werden
