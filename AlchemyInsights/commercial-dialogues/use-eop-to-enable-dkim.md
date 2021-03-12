---
title: Verwenden von Exchange Online PowerShell zum Aktivieren von DKIM für eine bestimmte Domäne
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736912"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Verwenden von Exchange Online PowerShell zum Aktivieren von DKIM für eine bestimmte Domäne

Wenn Sie die DKIM-DNS-Einträge nicht im Admin Center erstellen können, versuchen Sie es mit Exchange Online PowerShell. 

Führen Sie die folgenden Schritte aus, um einen DKIM-DNS-Eintrag mit Exchange Online PowerShell zu erstellen:

1. Öffnen Windows PowerShell als Administrator, und führen Sie die folgenden Befehle in der beschriebenen Reihenfolge aus:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Wenn Sie Probleme beim Herstellen einer Verbindung mit Exchange Online PowerShell haben, lesen Sie [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. Führen Sie nach der Verbindung mit Exchange Online PowerShell den folgenden Befehl aus:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Nachdem der obige Befehl erfolgreich ausgeführt wurde, führen Sie den folgenden Befehl aus, um die Exchange Online PowerShell-Sitzung zu beenden:

    `Remove-PSSession $Session` 



