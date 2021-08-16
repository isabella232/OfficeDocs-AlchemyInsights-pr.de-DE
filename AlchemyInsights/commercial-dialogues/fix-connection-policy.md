---
title: Beheben von Verbindungsrichtlinien
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988102"
---
# <a name="fix-connection-policy"></a>Beheben von Verbindungsrichtlinien

Die E-Mail wurde als sicher markiert und an den Posteingang des Benutzers übermittelt, da die sendende IP-Adresse in der Verbindungsfilterrichtlinie als sicher markiert wurde. Gehen Sie folgendermaßen vor, um die Richtlinie zu überprüfen:

1. Wechseln Sie zum [Office 365 Security & Compliance Center,](https://go.microsoft.com/fwlink/p/?linkid=2077143)und wechseln Sie dann zu   >    >  ["Antispamrichtlinie](https://go.microsoft.com/fwlink/?linkid=2101518)für die Bedrohungsverwaltung".
2. Wählen Sie auf der Registerkarte **"Benutzerdefiniert"** die **Verbindungsfilterrichtlinie** und dann **"Richtlinie bearbeiten"** aus.
3. Überprüfen Sie die Liste zugelassener **IP-Adressen.** Überprüfen Sie, ob **Tresor Liste** aktiviert ist.

    > [!NOTE]
    > Microsoft hat verschiedene Quellen von Drittanbietern mit vertrauenswürdigen Absendern abonniert. Wenn **Tresor Liste** aktiviert ist, werden diese vertrauenswürdigen Absender nicht versehentlich als Spam gekennzeichnet. Ich empfehlen, diese Option auszuwählen, da dadurch die Anzahl falsch positiver Nachrichten (gute E-Mails, die als Spam klassifiziert werden) reduziert wird, die Sie erhalten.
