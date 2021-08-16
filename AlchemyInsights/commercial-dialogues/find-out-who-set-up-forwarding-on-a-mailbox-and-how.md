---
title: Erfahren Sie, wer die Weiterleitung für ein Postfach eingerichtet hat und wie
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988199"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Erfahren Sie, wer die Weiterleitung für ein Postfach eingerichtet hat und wie

Wenn die externe Weiterleitung für ein Postfach festgelegt wurde, wird die Aktivität als Teil des Cmdlets Set-Mailbox überwacht. So finden Sie die Aktivität im Überwachungsprotokoll:

1. Wechseln Sie zum [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Wählen Sie  >  **"Überwachungsprotokollsuche durchsuchen" aus.**
    > [!NOTE]
    > Wenn Sie einen Hinweis sehen, dass Sie die Überwachung aktivieren müssen, fahren Sie fort, und aktivieren Sie sie jetzt. Wenn dieses Feature nicht aktiviert ist, können Suchergebnisse keine Daten aus früheren Datumsangaben abrufen.
1. Stellen Sie sicher, dass das Feld **"Aktivitäten"** auf **"Ergebnisse für alle Aktivitäten anzeigen"** festgelegt ist (Standardeinstellung). Geben Sie den Datumsbereich an. Sie müssen keinen Benutzernamen angeben.
1. Wählen Sie **Suchen** aus. Die Aktivitäten werden unter **Ergebnisse** angezeigt.
1. Wählen Sie **"Filterergebnisse"** aus, und geben **Sie "Set-mailbox"** in das Feld **"Aktivitätsfilter"** ein. Dadurch werden alle **Set-Mailbox-Aktivitäten** zurückgegeben.
1. Um die Details anzuzeigen, wählen Sie eine Aktivität aus, und wählen Sie dann **weitere Informationen** aus. Unter **"Parameter"** sehen Sie die Weiterleitungs-E-Mail-Adresse, die für das Postfach festgelegt wurde. Die **UserID** stellt den Benutzer dar, der die externe Weiterleitung für das Postfach eingerichtet hat.
Weitere Informationen finden Sie unter [Durchsuchen des Office 365 Überwachungsprotokolls, um häufige Szenarien zu beheben.](https://go.microsoft.com/fwlink/?linkid=2103944)