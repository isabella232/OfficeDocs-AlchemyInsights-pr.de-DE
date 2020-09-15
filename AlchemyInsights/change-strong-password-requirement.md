---
title: Ändern der Anforderung für sicheres Kennwort
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
- "9000105"
- "1600"
ms.openlocfilehash: d888f4a208ccbc6f54469f5e1eb88f9f4197e5c9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47681871"
---
# <a name="change-strong-password-requirement"></a>Ändern der Anforderung für sicheres Kennwort

Microsoft erfordert standardmäßig sichere Kennwörter. 

Mithilfe von PowerShell können Sie mit dem folgenden Befehl sichere Kennwörter für bestimmte Benutzer deaktivieren:<br>
*Gruppe-MsolUser – userPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*

- [Weitere Informationen zur Kennwortrichtlinie](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Herstellen einer Verbindung mit Microsoft 365 mit PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Weitere Informationen zu PowerShell-MsolUser-Befehlen](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
