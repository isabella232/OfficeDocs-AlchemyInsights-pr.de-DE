---
title: Wiederherstellen eines gelöschten Formulars
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2547"
- "9000672"
ms.openlocfilehash: 48018accc23a504c34b5469c198d6f29929d25c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809474"
---
# <a name="restore-a-deleted-form"></a>Wiederherstellen eines gelöschten Formulars

Wenn Sie ein Formular versehentlich in Microsoft Forms gelöscht haben, können Sie es wiederherstellen. Melden Sie sich bei Microsoft Forms als Besitzer des gelöschten Formulars an. Wählen Sie **den Papierkorb** aus, wählen Sie dann das Formular aus, das Sie wiederherstellen möchten, und wählen Sie **Wiederherstellen aus.** Wählen Sie nach der Wiederherzustellenden Option **den Seitenpfeil Zurück zu meinem Formular** aus.

Nur der Besitzer des Formulars kann es wiederherstellen. Wenn das Konto des Formularbesitzers deaktiviert oder aus dem Mandanten entfernt wurde, kann nur der globale Administrator das Formular wiederherstellen. Der globale Administrator muss über eine Formularlizenz verfügen, um eine Wiederherstellung durchführen zu können. Nur Formulare, die innerhalb von 30 Tagen nach dem Deaktivieren oder Entfernen des Benutzerkontos aus dem Mandanten erstellt wurden, können wiederhergestellt werden.

Wenn Sie der globale Administrator des Mandanten sind und ein Formular von einem gelöschten oder deaktivierten Konto wiederherstellen möchten, ersetzen Sie [E-Mail-Adresse] durch die E-Mail-Adresse des gelöschten oder deaktivierten Benutzers in der folgenden URL: **https://forms.office.com/Pages/delegatepage.aspx?originalowner= [E-Mail-Adresse]** Wenn Ihre E-Mail-Adresse z. B. johndoe@contoso.com ist, ist die URL: **https://forms.office.com/Pages/delegatepage.aspx?originalowner=johndoe@contoso.com** . 

Sobald Sie Zugriff auf die gelöschten Formulare des Benutzers haben, wählen Sie das Formular aus, das Sie verschieben möchten, und wählen Sie dann **Weitere Formularaktionen**  >  **verschieben aus.**

Wenn Sie ein Formular wiederherstellen möchten, in dem es gelöscht wurde und der Benutzer aus der Organisation entfernt wurde, kann ein globaler Administrator den Benutzer wiederherstellen, das Kennwort für diesen Benutzer zurücksetzen und dann während der Anmeldung als dieser Benutzer auf das Formular zugreifen, um es zu einem anderen aktiven Benutzer zu verschieben. 