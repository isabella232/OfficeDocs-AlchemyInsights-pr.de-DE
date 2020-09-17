---
title: Zugriff auf Öffentliche Ordner nicht möglich
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
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812546"
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
      
    $true: Ermöglichen Sie Benutzern den Zugriff auf Öffentliche Ordner in Outlook  
      
    $false: Verhindern Sie den Zugriff von Benutzern auf Öffentliche Ordner in Outlook. Dies ist der Standardwert.  
        
2.  Gruppe-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Hinweis:** Dieses Verfahren kann Verbindungen nur mit Outlook Desktop für Windows-Clients steuern. Ein Benutzer kann weiterhin mithilfe von OWA oder Outlook für Mac auf Öffentliche Ordner zugreifen.
 
Weitere Informationen finden Sie unter [Ankündigung der Unterstützung für kontrollierte Verbindungen mit öffentlichen Ordnern in Outlook](https://aka.ms/controlpf).