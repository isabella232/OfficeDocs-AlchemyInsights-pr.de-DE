---
title: Zugriff auf Öffentliche Ordner nicht möglich
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959494"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook kann keine Verbindung zu öffentlichen Ordnern herstellen

Wenn der Zugriff auf Öffentliche Ordner nicht für wenige Benutzer funktioniert, versuchen Sie Folgendes:

Stellen Sie eine Verbindung mit Exo PowerShell her, und konfigurieren Sie die DefaultPublicFolderMailbox für das Problem Benutzerkonto so, dass Sie mit einem Konto in einem funktionierenden Benutzerkonto übereinstimmen.

Beispiel:

Get-Mailbox WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Festlegen-Postfach ProblemUser-DefaultPublicFolderMailbox \<-Wert aus dem vorherigen Befehls>

Warten Sie mindestens eine Stunde, bis die Änderung wirksam wird.