---
title: 126 Fehler beim Aufrufen eines Postfachs in OWA gefunden?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 9a8897767ebfebac5807116251634c615ef6767d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47706749"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Fehler beim Aufrufen eines Postfachs nicht gefunden in Outlook im Internet?

Wenn Sie Outlook im Internet verwenden und ein Postfach wegen eines Fehlers **nicht gefunden werden konnte** , hat das Konto, das Sie zum Herstellen einer Verbindung mit Outlook im Internet verwendet haben, keine Exchange Online Lizenz und daher ist dem Konto kein Postfach zugeordnet. Ihr Administrator kann Ihrem Konto eine Lizenz zuweisen, indem Sie die folgenden Schritte ausführen:

1. Öffnen Sie das [Microsoft 365 Admin Center](https://portal.office.com/adminportal/home#/homepage) , und wechseln Sie zu **aktive Benutzer** im Abschnitt **Benutzer** , und wählen Sie den Benutzer aus, der den Fehler sieht.

2. Wechseln Sie auf der Seite Benutzer, die geöffnet wird, zum Abschnitt **Lizenzen und apps** , wählen Sie den entsprechenden **Standort** Wert aus, und weisen Sie eine Lizenz zu, die Exchange Online enthält (erweitern Sie die Lizenz, um die Details anzuzeigen). Klicken Sie nach Abschluss des Vorgangs auf **Änderungen speichern**.
