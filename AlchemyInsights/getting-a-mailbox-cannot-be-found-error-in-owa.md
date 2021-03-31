---
title: 126 Fehler beim Abrufen eines Postfachs in OWA gefunden?
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
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426661"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Abrufen eines Postfachs nicht gefunden Fehler in Outlook im Web?

Wenn Sie Outlook im Web verwenden und ein **Postfach** nicht gefunden werden konnte, ist das Konto, das Sie zum Herstellen einer Verbindung mit Outlook im Web verwendet haben, nicht über eine Exchange Online-Lizenz, und daher ist dem Konto kein Postfach zugeordnet. Ihr Administrator kann Ihrem Konto eine Lizenz zuweisen, indem sie die folgenden Schritte ausführen:

1. Öffnen Sie [das Microsoft 365 Admin Center,](https://portal.office.com/adminportal/home#/homepage) und wechseln Sie im Abschnitt Benutzer zu Aktive Benutzer, und wählen Sie den Benutzer aus, dem der Fehler angezeigt wird.  

2. Wechseln Sie auf der geöffneten Benutzerseite zum Abschnitt Lizenzen und **Apps,** wählen Sie den entsprechenden **Standortwert** aus, und weisen Sie eine Lizenz zu, die Exchange Online enthält (erweitern Sie die Lizenz, um ihre Details anzuzeigen). Klicken Sie nach Abschluss des Vorgangs auf **Änderungen speichern**.

In einigen Fällen hilft das Entfernen und Erneute Zuweisen der Lizenz, wenn die Lizenz bereits einem Benutzerkonto zugewiesen ist, das Problem zu beheben und ordnungsgemäß im System bereitgestellt zu bekommen: 

- Überprüfen Sie, ob Ihre M365 Exchange Online -Abonnements (und andere, sofern Sie über ein Abonnement verfügen) aktuell sind und noch nicht abgelaufen sind.

Nachdem Sie sichergestellt haben, dass Ihr Abonnement nicht abgelaufen ist und dem Benutzerkonto eine gültige Lizenz zugewiesen wurde, kann es bis zu 24 Stunden dauern, bis die Lizenz bereitgestellt wurde, sodass Sie möglicherweise warten müssen, bis Ihr Problem behoben ist. Weitere Informationen finden Sie unter [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).