---
title: Festlegen von ClientAccessServerEnabled auf True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50509747"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Festlegen von ClientAccessServerEnabled auf True

Wenn Sie keine verschlüsselte E-Mail-Nachricht öffnen und stattdessen eine **rpmsg-Anlage** sehen können, führen Sie die folgenden Schritte aus:

1. Stellen Sie eine Verbindung mit Exchange Online PowerShell her.

> [!NOTE]
> Um eine Verbindung mit Exchange Online PowerShell herzustellen, müssen Sie sich mit einem globalen Administrator- oder Exchange-Administratorkonto anmelden.

   a. Öffnen Windows PowerShell, und führen Sie dann den folgenden Befehl aus: `$UserCredential = Get-Credential`
b. Geben Sie **im Windows PowerShell** Anmeldeinformationsanforderung Ihr Arbeits- oder Schulkonto und das Kennwort c ein. Klicken Sie auf **OK**. 

2. Führen Sie den folgenden Befehl aus, um eine neue Sitzung zu erstellen:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Führen Sie den folgenden Befehl aus:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Befehl `Get-IRMConfiguration` ausführen.

4. Überprüfen Sie die **Einstellung ClientAccessServerEnabled.** 

    a. Wenn **die Einstellung ClientAccessServerEnabled** auf **False festgelegt ist,** führen Sie das folgende Cmdlet aus: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Schließen Sie Ihre powershell-Sitzung immer mit dem folgenden Befehl: `Remove-PSSession $Session`

Weitere Informationen finden Sie unter [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

