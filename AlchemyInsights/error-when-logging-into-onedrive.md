---
title: 0x8004de40 fehler beim Starten von OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813651"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 fehler beim Starten von OneDrive

Wenn bei der Anmeldung bei OneDrive **0x8004de40** Fehler angezeigt wird, starten Sie den Computer neu, während sie mit Ihrer Arbeits- oder Schuldomäne verbunden sind. Wenn Sie diesen Fehler nach dem Neustart erhalten, versuchen Sie dies, während Sie mit Ihrer Arbeits- oder Schuldomäne verbunden sind:

1. Klicken Sie auf Start, und geben Sie **cmd** **oder** Eingabeaufforderung in das Suchfeld ein, klicken Sie mit der rechten Maustaste auf die Eingabeaufforderungs-App, und wählen Sie Als Administrator **ausführen aus.** Wenn Sie zur Eingabe eines Administratorkennworts oder einer Bestätigung aufgefordert werden, geben Sie das Kennwort ein, oder klicken Sie auf **Zulassen**.  

2. Geben Sie im Eingabeaufforderungsfenster **dsregcmd /leave ein,**  und warten Sie, bis der Befehl abgeschlossen ist. Geben Sie dann **dsregcmd /join ein,** und warten Sie, bis der Befehl abgeschlossen ist.
3. Starten Sie Ihren Computer neu.
