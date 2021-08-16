---
title: Suchen der IP-Adresse im Überwachungsprotokoll
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
ms.openlocfilehash: 5b58803719df700290f495cb2d2d6742f072420a2a1d393534ca165bb5a14fbb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54017131"
---
# <a name="find-the-ip-address-in-audit-log"></a>Suchen der IP-Adresse im Überwachungsprotokoll

1. Die IP-Adresse, die einer von einem Benutzer oder Administrator ausgeführten Aktivität entspricht, wird in den Überwachungsprotokollen angezeigt. Die Clientinformationen werden ebenfalls protokolliert. So identifizieren Sie die IP-Adresse:

1. Wechseln Sie zum [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Wählen Sie   >  **["Überwachungsprotokollsuche durchsuchen" aus.](https://go.microsoft.com/fwlink/?linkid=2103759)**
    > [!NOTE]
    > Wenn Sie einen Hinweis sehen, dass Sie die Überwachung aktivieren müssen, fahren Sie fort, und aktivieren Sie sie jetzt. Wenn dieses Feature nicht aktiviert ist, können Suchergebnisse keine Daten aus früheren Datumsangaben abrufen.
1. Wenn Sie an einer bestimmten Aktivität interessiert sind, wählen Sie sie aus der **Liste "Aktivitäten"** aus. andernfalls werden standardmäßig alle Aktivitäten für den ausgewählten Benutzer zurückgegeben. Beachten Sie, dass bestimmte Aktivitäten möglicherweise nicht für die Auswahl im Menü **"Aktivitäten"** verfügbar sind. Diese Überwachungselemente werden jedoch zurückgegeben, wenn **"Ergebnisse für alle Aktivitäten anzeigen"** ausgewählt ist (Standardeinstellung).
1. Geben Sie den Datumsbereich an, und wählen Sie im Feld **"Benutzer"** den Benutzernamen für den Benutzer aus, den Sie untersuchen möchten.
1. Wählen Sie **Suchen** aus. Die Aktivitäten werden unter **Ergebnisse** angezeigt. Sie können die IP-Adresse für jede Aktivität anzeigen.
1. Um Details anzuzeigen, wählen Sie eine Aktivität aus, und wählen Sie dann **weitere Informationen** aus.

Weitere Informationen finden Sie unter Durchsuchen des [Office 365 Überwachungsprotokolls, um allgemeine Szenarien zu behandeln.](https://go.microsoft.com/fwlink/?linkid=2103944)