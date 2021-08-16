---
title: 126 Fehler beim Abrufen eines Postfachs in OWA nicht gefunden?
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
ms.openlocfilehash: aca0371dad9ba43fa21b0df8e50f1b8ee536528af90d6bda401995c6e5796be4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54056489"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Fehlermeldung "Postfach nicht gefunden" in Outlook im Web erhalten?

Wenn Sie Outlook im Web verwenden und ein Postfach aufgrund eines **Fehlers nicht gefunden werden konnte,** verfügt das Konto, das Sie zum Herstellen einer Verbindung mit Outlook im Web verwendet haben, nicht über eine Exchange Online Lizenz, und daher ist dem Konto kein Postfach zugeordnet. Ihr Administrator kann Ihrem Konto eine Lizenz zuweisen, indem er die folgenden Schritte ausführt:

1. Öffnen Sie die [Microsoft 365 Admin Center,](https://portal.office.com/adminportal/home#/homepage) wechseln Sie im Abschnitt **"Benutzer"** zu **"Aktive Benutzer",** und wählen Sie den Benutzer aus, dem der Fehler angezeigt wird.

2. Wechseln Sie auf der geöffneten Benutzerseite zum Abschnitt **"Lizenzen und Apps",** wählen Sie den entsprechenden **Standortwert** aus, und weisen Sie eine Lizenz zu, die Exchange Online enthält (erweitern Sie die Lizenz, um ihre Details anzuzeigen). Klicken Sie nach Abschluss des Vorgangs auf **Änderungen speichern**.

Wenn die Lizenz in einigen Fällen bereits einem Benutzerkonto zugewiesen ist, hilft das Entfernen und erneute Zuweisen der Lizenz, das Problem zu beheben und im System ordnungsgemäß bereitzustellen: 

- Überprüfen Sie, ob Ihre M365-Exchange Online -Abonnements (und andere, sofern Vorhanden) aktuell sind und nicht vor kurzem abgelaufen sind.

Nachdem Sie sichergestellt haben, dass Ihr Abonnement nicht abgelaufen ist und dem Benutzerkonto eine gültige Lizenz zugewiesen wurde, kann es bis zu 24 Stunden dauern, bis die Lizenz bereitgestellt wurde. Daher müssen Sie möglicherweise warten, bis ihr Problem behoben ist. Weitere Informationen finden Sie unter [Zuweisen und Verwalten von Lizenzen.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)