---
title: Steuern des Zugriffs auf Öffentliche Ordner mit Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032557"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Steuern des Zugriffs auf Öffentliche Ordner mit Outlook

So steuern Sie, welche Benutzer über Outlook auf Öffentliche Ordner zugreifen können:

1. `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false` verwenden

$true: Ermöglichen Sie Benutzern den Zugriff auf Öffentliche Ordner in Outlook  
$false: Verhindern Sie den Zugriff von Benutzern auf Öffentliche Ordner in Outlook. Dies ist der Standardwert.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Hinweis: Mit diesem Verfahren können nur Verbindungen mit dem Outlook-Desktop für Windows-Clients gesteuert werden. Benutzer können weiterhin mit OWA oder Outlook für Mac auf Öffentliche Ordner zugreifen.

Weitere Informationen hierzu finden Sie unter [Kontrollierte Verbindungen zu Öffentlichen Ordnern in Outlook](https://aka.ms/controlpf).
