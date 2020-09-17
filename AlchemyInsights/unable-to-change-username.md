---
title: Benutzername (UserName) kann nicht geändert werden
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 76891b3abe156b736c3bb6da0f6cd1135346dbe2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798663"
---
# <a name="unable-to-change-username"></a>Benutzername (UserName) kann nicht geändert werden

In einigen Fällen werden UPN-Änderungen (UserPrincipalName) nicht in die Cloud übertragen. Möglicherweise erhalten Sie Validierungsfehler im Office 365-Portal oder können den Benutzernamen oder die E-Mail-Adresse nicht ändern. Um dieses Problem zu beheben, legen Sie "UserPrincipalName" mit diesem PowerShell-Befehl manuell fest.

**Beispiel: Umbenennen eines Benutzers**

PowerShellCopy

PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Mit diesem Befehl wird "davidc@contoso.com" in "davidchew@contoso.com" umbenannt.

Weitere Informationen finden Sie unter [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).