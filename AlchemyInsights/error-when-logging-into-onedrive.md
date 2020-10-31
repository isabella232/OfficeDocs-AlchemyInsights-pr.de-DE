---
title: 0x8004de40-Fehler beim Starten von OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/30/2020
ms.locfileid: "48815992"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40-Fehler beim Starten von OneDrive

Wenn beim Anmelden bei OneDrive ein Fehler **0x8004de40** angezeigt wird, starten Sie den Computer neu, während eine Verbindung mit ihrer Arbeits-oder Schul Domäne besteht. Wenn Sie diesen Fehler nach dem Neustart erhalten, versuchen Sie Folgendes, während Sie mit ihrer geschäftlichen oder schulischen Domäne verbunden sind:

1. Klicken Sie auf Start, und geben Sie **cmd** oder **Eingabeaufforderung**  in das Suchfeld ein, klicken Sie mit der rechten Maustaste auf die Eingabe Aufforderungs-APP, und wählen Sie  **als Administrator ausführen** aus. Wenn Sie zur Eingabe eines Administratorkennworts oder zur Bestätigung aufgefordert werden, geben Sie das Kennwort ein, oder klicken Sie auf **zulassen** .  

2. Geben Sie in das Eingabeaufforderungsfenster **dsregcmd/Leave**  ein, und warten Sie, bis der Befehl abgeschlossen ist. Geben Sie dann **dsregcmd/Join** ein, und warten Sie, bis der Befehl abgeschlossen ist.
3. Starten Sie den Computer neu.
