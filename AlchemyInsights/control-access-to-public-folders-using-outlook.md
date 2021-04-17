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
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816739"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Steuern des Zugriffs auf Öffentliche Ordner mit Outlook

So steuern Sie, welche Benutzer über Outlook auf Öffentliche Ordner zugreifen können:

1. `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false` verwenden

$true: Ermöglichen Sie Benutzern den Zugriff auf Öffentliche Ordner in Outlook  
$false: Verhindern Sie den Zugriff von Benutzern auf Öffentliche Ordner in Outlook. Dies ist der Standardwert.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Hinweis: Mit diesem Verfahren können nur Verbindungen mit dem Outlook-Desktop für Windows-Clients gesteuert werden. Benutzer können weiterhin mit OWA oder Outlook für Mac auf Öffentliche Ordner zugreifen.

Weitere Informationen hierzu finden Sie unter [Kontrollierte Verbindungen zu Öffentlichen Ordnern in Outlook](https://aka.ms/controlpf).
