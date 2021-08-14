---
title: Automatische Verschlüsselung bestimmter E-Mail-Nachrichten aus Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 74f9733196004fd7a78eeb290c948a9f35ac2a31b3c5b00bf82e44081aac8637
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988834"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Automatische Verschlüsselung bestimmter E-Mail-Nachrichten aus Office 365

1. Wählen Sie im [Exchange Admin Center](https://outlook.office365.com/ecp/)den **Nachrichtenfluss > Regeln** aus. 
2. Klicken Sie auf das Symbol **"Neu" (+),** und klicken Sie dann auf **"Office 365-Nachrichtenverschlüsselung und Rechteschutz auf Nachrichten anwenden".**
3. Geben Sie unter **"Name"** einen Namen für die Regel ein, z. B. *"Alle Nachrichten verschlüsseln".*
4. Wählen Sie unter **"Diese Regel anwenden, wenn"** die Option **[Auf alle Nachrichten anwenden]** aus. 
5. Klicken Sie neben dem Feld **Ausführen** auf **Auswählen .** 
6. Wählen Sie im Dropdownmenü der **RMS-Vorlage** **"Verschlüsseln"** aus, und klicken Sie dann auf **"OK".** (Wenn diese Option nicht angezeigt wird, bedeutet dies, dass Ihr Plan keine automatische Verschlüsselung umfasst. Aber Sie können es hinzufügen!)
7. Aktivieren Sie das Kontrollkästchen **"Diese Regel mit Schweregrad** überwachen", und wählen Sie dann die gewünschte Ebene aus. Wenn Ihr Unternehmen vertraglich verpflichtet ist, alle E-Mails verschlüsselt zu senden, wird empfohlen, die Stufe auf **"Hoch"** festzulegen.
8. Klicken Sie unter **"Modell für diese Regel auswählen"** auf **"Erzwingen".** 
9. Wählen Sie eine beliebige optionale Auswahl aus (aus einer Liste optionaler Auswahlen, die Sie an diesem Punkt treffen können, von denen viele der Einfachheit halber mit der Standardeinstellung übrig bleiben können).
10. Klicken Sie auf **Speichern**.

> [!IMPORTANT]
> Sie können jederzeit zurückkehren und diese Regel später bearbeiten.

Weitere Informationen zum Erstellen von Regeln für die Verschlüsselung finden Sie unter [Definieren von Nachrichtenflussregeln zum Verschlüsseln von E-Mail-Nachrichten in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

