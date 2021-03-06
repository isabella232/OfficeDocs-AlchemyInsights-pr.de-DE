---
title: Automatisches Verschlüsseln bestimmter E-Mail-Nachrichten aus Office 365
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50509916"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Automatisches Verschlüsseln bestimmter E-Mail-Nachrichten aus Office 365

1. Wählen Sie [im Exchange Admin Center](https://outlook.office365.com/ecp/)die Option **Nachrichtenfluss > Regeln aus.** 
2. Klicken Sie **auf das Symbol Neu (+),** und klicken Sie dann auf Office **365-Nachrichtenverschlüsselung und -rechteschutz auf Nachrichten anwenden.**
3. Geben Sie unter **Name** einen Namen für die Regel ein, z. *B. Alle Nachrichten verschlüsseln.*
4. Wählen **Sie unter Diese Regel anwenden, wenn** die Option **[Auf alle Nachrichten anwenden] aus.** 
5. Klicken Sie neben **dem Feld Gehen Sie wie folgt** auf Wählen Sie **eins aus.** 
6. Wählen Sie **im Dropdownmenü RMS-Vorlage** die Option **Verschlüsseln** aus, und klicken Sie dann auf **OK**. (Wenn diese Option nicht angezeigt wird, bedeutet dies, dass Ihr Plan keine automatische Verschlüsselung umfasst. Sie können sie jedoch hinzufügen!)
7. Aktivieren Sie das Kontrollkästchen Diese **Regel mit Schweregrad überwachen,** und wählen Sie dann die gewünschte Ebene aus. Wenn Ihr Unternehmen vertragliche Verpflichtungen zum Senden aller verschlüsselten E-Mails hat, empfiehlt es sich, die Stufe auf **Hoch zu setzen.**
8. Klicken **Sie unter Modell für diese Regel auswählen** auf **Erzwingen**. 
9. Wählen Sie eine beliebige optionale Auswahl (aus einer Liste der optionalen Auswahlen, die Sie an diesem Punkt treffen können, von denen viele der Einfachheit halber der Standardeinstellung erhalten bleiben können).
10. Klicken Sie auf **Speichern**.

> [!IMPORTANT]
> Sie können diese Regel später immer wieder bearbeiten.

Weitere Informationen zum Erstellen von Regeln für die Verschlüsselung finden Sie unter Definieren von Nachrichtenflussregeln zum Verschlüsseln von E-Mail-Nachrichten [in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

