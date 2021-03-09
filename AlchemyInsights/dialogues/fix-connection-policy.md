---
title: Fix connection policy
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568565"
---
# <a name="fix-connection-policy"></a>Fix connection policy

Die E-Mail wurde als sicher gekennzeichnet und an den Posteingang des Benutzers übermittelt, da die sendende IP-Adresse in der Verbindungsfilterrichtlinie als sicher gekennzeichnet wurde. Gehen Sie wie folgt vor, um die Richtlinie zu überprüfen:

1. Wechseln Sie zum [Office 365 Security & Compliance Center,](https://go.microsoft.com/fwlink/p/?linkid=2077143)und wechseln Sie dann zu **Bedrohungsverwaltungsrichtlinie**  >    >  [Antispam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Wählen Sie **auf** der Registerkarte Benutzerdefinierte Die **Verbindungsfilterrichtlinie** aus, und wählen Sie dann **Richtlinie bearbeiten aus.**
3. Überprüfen Sie die **Liste der zulässigen IP-Adressen.** Sehen Sie, **ob die Liste "Sicher"** aktiviert ist.

    > [!NOTE]
    > Microsoft hat verschiedene Quellen von Drittanbietern mit vertrauenswürdigen Absendern abonniert. Wenn **die Liste "Sicher"** aktiviert ist, werden diese vertrauenswürdigen Absender nicht fälschlicherweise als Spam gekennzeichnet. Ich empfehle, diese Option zu wählen, da dadurch die Anzahl falsch positiver Nachrichten (gute E-Mails, die als Spam klassifiziert werden) reduziert wird, die Sie erhalten.
