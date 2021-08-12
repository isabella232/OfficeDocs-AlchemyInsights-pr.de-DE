---
title: Read-Only für Wartungsnachricht bei dem Versuch, SharePoint oder OneDrive zu verwenden
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: edcdea2f5c0647b92c230dd1d86549173e72997fc885195cde688b3b17710a2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910545"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only für Wartungsnachricht bei dem Versuch, SharePoint oder OneDrive zu verwenden

Benutzer erhalten möglicherweise eine Meldung **"Schreibgeschützt für Wartung",** wenn sie versuchen, SharePoint oder OneDrive für eines der folgenden Szenarien zu verwenden. 

-   Eine geplante oder aktive Wartungsaktivität.  Suchen Sie nach diesen, indem Sie zum [Nachrichtencenter](https://portal.office.com/adminportal/home#/messagecenter)navigieren.
-   Ein Aktiver Dienstvorfall mit hoher Priorität, der möglicherweise auftritt. Suchen Sie nach Empfehlungen/Vorfällen, indem Sie zu [Dienststatus](https://portal.office.com/adminportal/home#/servicehealth)navigieren.
-   Ein kleines Wiederherstellungsszenario für die automatische Wiederherstellung, das aufgrund unerwarteter Ereignisse auf den Servern auftreten könnte, die möglicherweise weniger als 30 Minuten dauern. 
    
    Es gibt keine Nachrichtencenter- oder Dienststatusbeiträge für diese geringfügigen Wiederherstellungen, aber Sie sollten sehr bald wieder zur Normalität zurückkehren.

In sehr wenigen Fällen haben wir festgestellt, dass eines der drei oben aufgeführten Szenarien die Ursache war, und der Dienst wurde wiederhergestellt, aber der Browsercache des Benutzers wurde nicht gelöscht.

Versuchen Sie, den Browsercache zu löschen, bevor Sie zur Website navigieren.

1. Wählen Sie in Ihrem Microsoft Edge Browser **Einstellungen** und dann **"Datenschutz und Sicherheit"** aus.
2. Wählen Sie unter **"Browser löschen"** die Option **aus, was gelöscht werden soll.**
3. Wählen Sie **Cookies und gespeicherte Websitedaten** aus, und wählen Sie **"Löschen"** aus.

>[!Note] 
> Diese Schritte können sich unterscheiden, wenn Sie andere Browser wie Mozilla Firefox oder Google Chrome verwenden.

>[!Note] 
> Eine weitere Möglichkeit besteht darin, Ihre SharePoint Website oder OneDrive in einem neuen InPrivate-Fenster zu öffnen.