---
title: Steuern des Zugriffs auf Öffentliche Ordner mit Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: b04e09f5110266d59db82e25cfda1835779fd4b7
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406571"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Steuern des Zugriffs auf Öffentliche Ordner mit Outlook

So steuern Sie, welche Benutzer über Outlook auf Öffentliche Ordner zugreifen können:

1. `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false` verwenden

$true: Ermöglichen Sie Benutzern den Zugriff auf Öffentliche Ordner in Outlook  
$false: Verhindern Sie den Zugriff von Benutzern auf Öffentliche Ordner in Outlook. Dies ist der Standardwert.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Hinweis: Mit diesem Verfahren können nur Verbindungen mit dem Outlook-Desktop für Windows-Clients gesteuert werden. Benutzer können weiterhin mit OWA oder Outlook für Mac auf Öffentliche Ordner zugreifen.

Weitere Informationen hierzu finden Sie unter [Kontrollierte Verbindungen zu Öffentlichen Ordnern in Outlook](https://aka.ms/controlpf).
