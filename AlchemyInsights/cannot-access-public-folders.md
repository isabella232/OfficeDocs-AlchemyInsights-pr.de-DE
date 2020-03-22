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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891748"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook kann keine Verbindung zu öffentlichen Ordnern herstellen

Wenn der Zugriff auf Öffentliche Ordner für einige Benutzer nicht funktioniert, versuchen Sie Folgendes:

Stellen Sie eine Verbindung mit Exo PowerShell her, und konfigurieren Sie den Parameter DefaultPublicFolderMailbox für das Problem Benutzerkonto so, dass er mit dem Parameter eines funktionierenden Benutzerkontos übereinstimmt.

Beispiel:

Get-Mailbox WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Festlegen-Postfach ProblemUser-DefaultPublicFolderMailbox \<-Wert aus dem vorherigen Befehls>

Warten Sie mindestens eine Stunde, bis die Änderung wirksam wird.

Wenn das Problem weiterhin besteht, führen Sie die folgenden [Schritte](https://aka.ms/pfcte) aus, um Probleme mit dem Zugriff auf Öffentliche Ordner mithilfe von Outlook zu beheben.