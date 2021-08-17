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
ms.openlocfilehash: 9094dcdc4507f52da1dd7c95f83aa98bab1446639d2d9f52eb3a7bc849dc183c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57888405"
---
# <a name="fix-connection-policy"></a>Beheben von Verbindungsrichtlinien

Die E-Mail wurde als sicher markiert und an den Posteingang des Benutzers übermittelt, da die Quell-IP-Adresse in der Standardverbindungsfilterrichtlinie als sicher markiert wurde. Führen Sie die folgenden Schritte aus, um die Richtlinie zu überprüfen:

1. Wechseln Sie im Microsoft 365 Defender-Portal unter <https://security.microsoft.com/> zu **E-Mail-& Richtlinien** für die Zusammenarbeit & Richtlinien für \>  \> **Bedrohungsregeln** \> **Antispam** im Abschnitt **"Richtlinien".**

   Wechseln Sie direkt zur Seite **Antispamrichtlinien**, verwenden Sie <https://security.microsoft.com/antispam>.

2. Wählen Sie auf der Seite **"Antispamrichtlinien"** die Richtlinie namens **Verbindungsfilterrichtlinie (Standard)** aus, indem Sie auf den Namen der Richtlinie klicken.

3. Klicken Sie im angezeigten Flyout "Details" im Abschnitt **"Verbindungsfilterung"** auf **"Verbindungsfilterrichtlinie bearbeiten".**

4. Überprüfen Sie die Einträge im Abschnitt **"Nachrichten immer zulassen" aus dem folgenden Abschnitt "IP-Adressen" oder "Adressbereich",** und überprüfen Sie, ob **"Sichere Liste aktivieren"** ausgewählt ist.

   > [!NOTE]
   > Microsoft hat verschiedene Quellen von Drittanbietern mit vertrauenswürdigen Absendern abonniert. Wenn die sichere Liste aktiviert ist, werden diese vertrauenswürdigen Absender nicht versehentlich als Spam gekennzeichnet. Wir empfehlen, diese Option auszuwählen, da dadurch die Anzahl falsch positiver Nachrichten (gute E-Mails, die als Spam klassifiziert werden) reduziert wird, die Sie erhalten.

Weitere Informationen finden Sie unter [Konfigurieren der Richtlinie für Verbindungsfilter](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy).
