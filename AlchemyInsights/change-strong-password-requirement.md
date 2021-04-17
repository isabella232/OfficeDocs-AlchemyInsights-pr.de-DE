---
title: Ändern der Anforderung für starke Kennwörter
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
- "9000105"
- "1600"
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818467"
---
# <a name="change-strong-password-requirement"></a>Ändern der Kennwortanforderung für starke Kennwörter

Microsoft benötigt standardmäßig sichere Kennwörter.

Mithilfe von PowerShell können Sie sichere Kennwörter für bestimmte Benutzer mit den folgenden Befehlen deaktivieren:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Verwenden Sie zum Deaktivieren von starken Kennwörtern für alle Benutzer:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Weitere Informationen zur Kennwortrichtlinie](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Herstellen einer Verbindung mit Microsoft 365 mit PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Weitere Informationen zu PowerShell-MsolUser-Befehlen](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
