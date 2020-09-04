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
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341402"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook kann keine Verbindung zu öffentlichen Ordnern herstellen

Wenn der Zugriff auf Öffentliche Ordner für einige Benutzer nicht funktioniert, versuchen Sie Folgendes:

Stellen Sie eine Verbindung mit Exo PowerShell her, und konfigurieren Sie den Parameter DefaultPublicFolderMailbox für das Problem Benutzerkonto so, dass er mit dem Parameter eines funktionierenden Benutzerkontos übereinstimmt.

Beispiel:

Get-Mailbox WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Festlegen-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

Warten Sie mindestens eine Stunde, bis die Änderung wirksam wird.

Wenn das Problem weiterhin besteht, führen Sie die folgenden [Schritte](https://aka.ms/pfcte) aus, um Probleme mit dem Zugriff auf Öffentliche Ordner mithilfe von Outlook zu beheben.
 
**So steuern Sie, welche Benutzer mit Outlook auf Öffentliche Ordner zugreifen können**:

1.  Verwenden Sie die $true oder $false von festlegen-CASMailbox <mailboxname> -PublicFolderClientAccess  
      
    $true: Benutzern den Zugriff auf Öffentliche Ordner in Outlook ermöglichen  
      
    $false: verhindern des Benutzerzugriffs auf Öffentliche Ordner in Outlook. Dies ist der Standardwert.  
        
2.  Gruppe-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Hinweis:** Dieses Verfahren kann Verbindungen nur mit Outlook Desktop für Windows-Clients steuern. Ein Benutzer kann weiterhin mithilfe von OWA oder Outlook für Mac auf Öffentliche Ordner zugreifen.
 
Weitere Informationen finden Sie unter [Ankündigung der Unterstützung für kontrollierte Verbindungen mit öffentlichen Ordnern in Outlook](https://aka.ms/controlpf).