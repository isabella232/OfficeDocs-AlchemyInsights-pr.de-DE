---
title: Schreibgeschützt für Wartungs Nachrichten beim Versuch, SharePoint oder OneDrive zu verwenden
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620722"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Schreibgeschützt für Wartungs Nachrichten beim Versuch, SharePoint oder OneDrive zu verwenden

Benutzer erhalten möglicherweise eine **schreibgeschützte Nachricht für die Wartung** , wenn Sie versuchen, SharePoint oder OneDrive für eines der folgenden Szenarien zu verwenden. 

-   Eine geplante oder aktive Wartungs Aktivität.  Überprüfen Sie diese, indem Sie zum [Nachrichten Center](https://portal.office.com/adminportal/home#/messagecenter)navigieren.
-   Ein aktiver Dienst Vorfall mit hoher Priorität, der möglicherweise auftritt. Suchen Sie nach Warnungen/Vorfällen, indem Sie zum [Dienststatus](https://portal.office.com/adminportal/home#/servicehealth)navigieren.
-   Ein kleines Wiederherstellungsszenario, das aufgrund unerwarteter Ereignisse auf den Servern möglicherweise nicht mehr als 30 Minuten dauern kann. 
    
    Es gibt keine Nachrichten Center-oder Dienst Integritäts Beiträge für diese kleinen Wiederherstellungen, aber Sie sollten bald wieder ganz normal sein.

In sehr seltenen Fällen haben wir festgestellt, dass eines der drei oben aufgelisteten Szenarien die Ursache war, und der Dienst wurde wiederhergestellt, aber der Browsercache für Benutzer wurde nicht gelöscht.

Versuchen Sie, den Browsercache zu löschen, bevor Sie zur Website navigieren.

1. Wählen Sie in Ihrem Microsoft Edge-Browser **Einstellungen**aus, und wählen Sie dann **Datenschutz und Sicherheit**aus.
2. Wählen Sie unter **Browser löschen** **die Option zu Lösch**Ende Elemente auswählen aus.
3. Wählen Sie **Cookies und gespeicherte Website Daten**aus, und wählen Sie **Löschen**aus.

>[!Note] 
> Diese Schritte können unterschiedlich sein, wenn Sie andere Browser wie Mozilla Firefox oder Google Chrome verwenden.

>[!Note] 
> Eine weitere Option besteht darin, Ihre SharePoint-Website oder OneDrive in einem neuen InPrivate-Fenster zu öffnen.