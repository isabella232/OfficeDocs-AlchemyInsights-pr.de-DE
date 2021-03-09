---
title: Senden einer E-Mail-Nachricht durch Angabe der Netzwerknachrichten-ID
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
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552358"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a>Senden einer E-Mail-Nachricht durch Angabe der Netzwerknachrichten-ID

1. Wählen Sie **im Flyout** Neue Übermittlung die Option **E-Mail** und **Netzwerknachrichten-ID aus.**
2. Führen Sie die folgenden Schritte aus, um die Nachrichten-ID für eine E-Mail-Nachricht in Outlook zu finden:
    1. Doppelklicken Sie auf die E-Mail-Nachricht, um sie zu öffnen.
    1. Wählen **Sie**  >  **Dateieigenschaften aus.**
    1. Öffnen Sie Editor oder ein **leeres** Word-Dokument, und kopieren Und fügen Sie dann den Inhalt aus dem Feld Internetkopfzeilen in das geöffnete Dokument ein, um eine bessere Sichtbarkeit zu erhalten.
    1. Suchen Sie **das Feld X-MS-Exchange-Organization-Network-Message-Id.** Der Wert nach **:** ist die ID, die Sie für Ihre Übermittlung benötigen.
3. Wählen **Sie unter Empfänger** die Option Alle auswählen aus, wenn die E-Mail im Junk-E-Mail-Ordner für alle Empfänger dieser E-Mail gelandet **ist.** Wenn nicht, wählen Sie nur den Benutzer aus, der das Problem gemeldet hat.
4. Geben **Sie unter** Übermittlungsgrund an, wenn Sie Die Option Hätte blockiert werden sollen, an, ob die Nachricht als **Spam,** **Phishing** oder **Schadsoftware** blockiert werden soll, und wählen Sie dann **Absenden aus.** 

Weitere Informationen finden Sie unter Übermitteln von verdächtigem [Spam, Phishing, URLs](https://go.microsoft.com/fwlink/?linkid=2101479)und Dateien an Microsoft zum Scannen.
