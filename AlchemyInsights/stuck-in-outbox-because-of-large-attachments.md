---
title: Hängen im Postausgang aufgrund großer Anlagen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241251"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Beheben von Nachrichten, die im Postausgang hängen

Es wird empfohlen, dass Sie zunächst das Szenario ["Ich habe Probleme beim Senden, empfangen oder finden von e-Mail-Nachrichten"](https://aka.ms/SaRA-OutlookSendReceive) im [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) -Tool durchführen.

Wenn eine Nachricht in Ihrem Postausgang feststeht, ist die wahrscheinlichste Ursache eine große Anlage oder die Option "sofort bei Verbindung senden" ist nicht aktiviert.

**Entfernen der großen Anlage**

1. Wählen Sie in Outlook **senden/empfangen** > **Arbeiten offline**aus. 
2. Wählen Sie im Navigationsbereich die Option **Postausgang**aus. Von hier aus haben Sie folgende Möglichkeiten: 
    - Löschen Sie die Nachricht (Wählen Sie Sie aus, und wählen Sie dann **Löschen**aus).
    - Ziehen Sie die Nachricht in den Ordner Entwürfe, doppelklicken Sie darauf, um Sie zu öffnen, und entfernen Sie die Anlage, wählen Sie Sie aus, und wählen Sie dann **Löschen**aus.
3. Wenn Sie eine Fehlermeldung erhalten, die besagt, dass Outlook versucht, die Nachricht zu übermitteln, schließen Sie Outlook. Es kann ein paar Augenblicke dauern, bis das Programm beendet ist. Wenn Outlook nicht geschlossen wird, drücken Sie STRG + ALT + ENTF, und klicken Sie dann auf **Task-Manager starten**. Wählen Sie im Task-Manager die Registerkarte **Prozesse** aus, Scrollen Sie nach unten zu Outlook. exe, und wählen Sie **Prozess beenden**aus.
4. Nachdem Outlook geschlossen wurde, starten Sie es neu, und wiederholen Sie die Schritte 2 und 3. 
5. Nachdem Sie die Anlage entfernt haben, klicken Sie auf **senden/empfangen** > **Arbeiten offline** , um die Online Arbeit fortzusetzen. 

Nachrichten werden auch im Postausgang festgehalten, wenn Sie auf **senden**klicken, aber keine Verbindung hergestellt ist. Klicken Sie auf **senden/empfangen** und sehen Sie sich die Schaltfläche **Offline arbeiten** an. Wenn es blau ist, sind Sie getrennt. Klicken Sie darauf, um eine Verbindung herzustellen (die Schaltfläche wird weiß), und klicken Sie auf **Alle senden**.
 
**Sofortnachrichten senden bei Verbindung aktivieren**
 
1. Klicken Sie auf der Registerkarte Datei auf **Optionen**.

2. Klicken Sie im Dialogfeld Outlook-Optionen auf **erweitert**.

3. Klicken Sie im Abschnitt senden und empfangen auf, um **bei einer Verbindung sofort senden**zu aktivieren. Klicken Sie auf **OK**.
 
Ausführliche Informationen finden Sie unter:
- [Video: senden oder Löschen einer Stuck-e-Mail](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [E-Mail-Nachrichten bleiben im Ordner Postausgang, bis Sie einen Sende-oder Empfangsvorgang in Outlook manuell initiieren](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
