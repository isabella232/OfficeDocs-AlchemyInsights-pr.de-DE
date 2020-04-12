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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232629"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>Beheben von Nachrichten, die im Postausgang hängen

Es wird empfohlen, dass Sie zunächst das Szenario ["Ich habe Probleme beim Senden, empfangen oder finden von e-Mail-Nachrichten"](https://aka.ms/SaRA-OutlookSendReceive) vom [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) -Tool auf dem betroffenen Computer aus starten.

Wenn eine Nachricht in Ihrem Postausgang feststeht, ist die wahrscheinlichste Ursache eine große Anlage oder die Option "sofort bei Verbindung senden" ist nicht aktiviert.

**Entfernen der großen Anlage**

1. Klicken Sie auf **senden/empfangen** > **Arbeiten offline**. 
2. Klicken Sie im Navigationsbereich auf **Postausgang**. Von hier aus haben Sie folgende Möglichkeiten: 
    - Löschen Sie die Nachricht. Wählen Sie Sie einfach aus, und klicken Sie auf **Löschen**.
    - Ziehen Sie die Nachricht in den **Ordner Entwürfe**, doppelklicken Sie auf, um die Nachricht zu öffnen, und löschen Sie die Anlage (Klicken Sie darauf, und klicken Sie auf **Löschen**).
3. Wenn ein Fehler besagt, dass Outlook versucht, die Nachricht zu übermitteln, schließen Sie Outlook. Es kann ein paar Augenblicke dauern, bis das Programm beendet ist. Wenn Outlook nicht geschlossen wird, drücken Sie **STRG + ALT + ENTF** , und klicken Sie auf **Task-Manager starten**. Wählen Sie im Task-Manager die Registerkarte **Prozesse** aus, Scrollen Sie nach unten zu Outlook. exe, und klicken Sie dann auf **Prozess beenden**.
4. Nachdem Outlook geschlossen wurde, starten Sie Outlook neu, und wiederholen Sie die Schritte 2-3. 
5. Nachdem Sie die Anlage entfernt haben, klicken Sie auf **senden/empfangen** > **Arbeiten offline** , um die Auswahl der Schaltfläche aufzuheben und die Online Arbeit fortzusetzen. 

Nachrichten werden auch im Postausgang festgehalten, wenn Sie auf **senden**klicken, aber keine Verbindung hergestellt ist. Klicken Sie auf **senden/empfangen** und sehen Sie sich die Schaltfläche **Offline arbeiten** an. Wenn es blau ist, sind Sie getrennt. Klicken Sie darauf, um eine Verbindung herzustellen (die Schaltfläche wird weiß), und klicken Sie auf **Alle senden**.
 
**Sofortnachrichten senden bei Verbindung aktivieren**
 
1. Klicken Sie auf der Registerkarte Datei auf **Optionen**.

2. Klicken Sie im Dialogfeld Outlook-Optionen auf **erweitert**.

3. Klicken Sie im Abschnitt senden und empfangen auf, um **bei einer Verbindung sofort senden**zu aktivieren. Klicken Sie auf **OK**.
 
Ausführliche Informationen finden Sie unter:
- [Video: senden oder Löschen einer Stuck-e-Mail](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [E-Mail-Nachrichten bleiben im Ordner Postausgang, bis Sie einen Sende-oder Empfangsvorgang in Outlook manuell initiieren](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
