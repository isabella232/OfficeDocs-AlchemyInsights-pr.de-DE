---
title: Zugriff auf öffentliche Ordner nicht möglich
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
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819511"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook kann keine Verbindung mit öffentlichen Ordnern herstellen

Wenn der Zugriff auf öffentliche Ordner für einige Benutzer nicht funktioniert, versuchen Sie Folgendes:

Stellen Sie eine Verbindung mit EXO PowerShell ein, und konfigurieren Sie den Parameter DefaultPublicFolderMailbox für das Problembenutzerkonto so, dass er mit dem Parameter für ein funktionierendes Benutzerkonto übereinstimmen kann.

Beispiel:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Warten Sie mindestens eine Stunde, bis die Änderung wirksam wird.

Wenn das Problem weiterhin bestehen bleibt, führen Sie dieses Verfahren aus, [um](https://aka.ms/pfcte) Probleme mit dem Zugriff auf öffentliche Ordner mithilfe von Outlook zu beheben.
 
**So steuern Sie, welche Benutzer über Outlook auf öffentliche Ordner zugreifen können:**

1.  Verwenden Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true oder $false  
      
    $true: Ermöglichen Sie Benutzern den Zugriff auf Öffentliche Ordner in Outlook  
      
    $false: Verhindern Sie den Zugriff von Benutzern auf Öffentliche Ordner in Outlook. Dies ist der Standardwert.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Hinweis** Dieses Verfahren kann nur Verbindungen mit Outlook Desktop für Windows-Clients steuern. Ein Benutzer kann weiterhin über OWA oder Outlook für Mac auf öffentliche Ordner zugreifen.
 
Weitere Informationen finden Sie unter [Ankündigung der Unterstützung für kontrollierte Verbindungen mit öffentlichen Ordnern in Outlook](https://aka.ms/controlpf).