---
title: Automatisches Verschieben von E-Mail-Nachrichten in das Archivpostfach
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
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736776"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Automatisches Verschieben von E-Mail-Nachrichten in das Archivpostfach

So richten Sie eine Richtlinie ein, um die alten E-Mails eines Benutzers automatisch in das Archivpostfach zu verschieben:

1. Wechseln Sie [**zu Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143)Data Governance Archive, um zu überprüfen, ob ein Archivpostfach für den Benutzer aktiviert  >    >   wurde. Falls nicht, klicken Sie im **Warnfeld** auf Aktivieren **und** dann auf Ja.
2. Wechseln Sie [**zu Exchange Admin Center > Compliance management > Aufbewahrungstags**](https://go.microsoft.com/fwlink/?linkid=2059104).
3. Wählen Sie das Symbol + und dann **automatisch auf das gesamte Postfach anwenden aus.**
4. Weisen Sie dem Aufbewahrungstag einen Namen zu, und wählen **Sie In Archiv verschieben aus.** Geben Sie für den Aufbewahrungszeitraum die zeit ein, die Sie möchten, z. B. 90 Tage. Klicken Sie auf **Speichern**.
5. Erstellen Sie nun eine Aufbewahrungsrichtlinie: Wählen Sie **Aufbewahrungsrichtlinien** aus, wählen Sie das Symbol aus, um eine neue Richtlinie hinzuzufügen.
6. Weisen Sie der Aufbewahrungsrichtlinie einen Namen zu, und klicken Sie dann auf und scrollen Sie, um das gerade erstellte Aufbewahrungstag zu finden und hinzuzufügen. Klicken Sie auf **Speichern**.
7. Wenden Sie schließlich die Aufbewahrungsrichtlinie auf das Postfach des Benutzers an: Wechseln Sie noch im Exchange Admin Center zu  >  **Empfängerpostfächer**. Wählen Sie alle Benutzer aus, auf die Sie die Richtlinie anwenden möchten, und klicken Sie dann **auf Bearbeiten** (das Stiftsymbol).
8. Klicken Sie im Dialogfeld auf **Postfachfeatures**. Wenden **Sie unter** Aufbewahrungsrichtlinie die Richtlinie an, die Sie gerade > Speichern erstellt **haben.**
9. Anweisungen zum Anwenden der Richtlinie auf alle Benutzer finden Sie unter [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).
