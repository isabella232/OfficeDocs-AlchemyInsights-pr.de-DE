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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464615"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Erfahren Sie, wer die Weiterleitung für ein Postfach eingerichtet hat und wie

Wenn die externe Weiterleitung für ein Postfach festgelegt wurde, wird die Aktivität im Rahmen des cmdlets Set-Mailbox überwacht. So finden Sie die Aktivität im Überwachungsprotokoll:

1. Wechseln Sie zum [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Wählen **Sie Suche** >  **Überwachungsprotokollsuche aus.**
    > [!NOTE]
    > Wenn Sie eine Benachrichtigung sehen, dass Sie die Überwachung aktivieren müssen, fahren Sie mit der Überwachung voran, und aktivieren Sie sie jetzt. Wenn dieses Feature nicht aktiviert ist, können Suchergebnisse keine Daten aus früheren Datumsangaben ziehen.
1. Stellen Sie **sicher, dass das** Feld Aktivitäten auf Ergebnisse für alle Aktivitäten anzeigen festgelegt ist (Standardeinstellung).  Geben Sie den Datumsbereich an. Sie müssen keinen Benutzernamen angeben.
1. Wählen Sie **Suchen aus.** Die Aktivitäten werden unter **Ergebnisse angezeigt.**
1. Wählen **Sie Ergebnisse filtern** aus, und geben Sie dann **Set-mailbox** in das Feld **Aktivitätsfilter** ein. Dadurch werden alle **Set-Mailbox-Aktivitäten** zurückgegeben.
1. Wählen Sie zum Anzeigen der Details eine Aktivität aus, und wählen Sie dann **Weitere Informationen aus.** Unter **Parametern** wird die Weiterleitungs-E-Mail-Adresse angezeigt, die für das Postfach festgelegt wurde. Die **UserID** stellt den Benutzer dar, der die externe Weiterleitung für das Postfach eingerichtet hat.
Weitere Informationen finden Sie unter [Durchsuchen des Office 365-Überwachungsprotokolls zur Problembehandlung gängiger Szenarien.](https://go.microsoft.com/fwlink/?linkid=2103944)