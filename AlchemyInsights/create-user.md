---
title: Benutzer erstellen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: afba00ffc6ba082606e0071b41e2917b11e6a39d61cd0df7e468f0238f2ed8e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118743"
---
# <a name="create-user"></a>Benutzer erstellen

**Ankündigung:**

- [Veralteter WebView-Anmeldesupport von Google ab dem 4. Januar 2021.](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Testen Sie, ob Ihre Apps möglicherweise betroffen sind, indem Sie die [Google-Anleitungen zum](https://go.microsoft.com/fwlink/?linkid=2157323) Testen der Kompatibilität befolgen.
- Stellen Sie sicher, dass Sie die Systemwebansicht oder den Systembrowser verwenden, wenn Sie Ihre Benutzer mit Google-Consumerkonten anmelden. Weitere Informationen finden Sie unter [Probleme bei der Anmeldung bei Anwendungen (nur Chrome-Browser)](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**Ich kann keinen neuen Benutzer in meinem Azure AD-Verzeichnis erstellen**

1. Vergewissern Sie sich, dass Sie berechtigt sind, einen neuen Standardbenutzer zu erstellen. Nur die Rolle "Globaler Administrator" oder "Benutzeradministrator" in Azure Active Directory (AD) kann einen neuen Standardbenutzer erstellen. Wenn Sie keine dieser Rollen besitzen, bitten Sie einen Administrator, Sie einer dieser Rollen hinzuzufügen oder das neue Benutzerkonto für Sie zu erstellen.
1. Stellen Sie sicher, dass der Benutzername zu der Domäne gehört, die in Azure AD verifiziert wurde. Wenn es in Azure AD keine verifizierten benutzerdefinierten Domänennamen gibt, können Sie Ihre anfängliche Azure AD-Domäne verwenden, welche mit "*.onmicrosoft.com" endet.
1. Stellen Sie sicher, dass der Benutzername zu einer Domäne gehört, die nicht mit Azure AD über Ihr lokales AD verbunden ist. Benutzer mit über lokale Umgebungen verbundenen Domänennamen können nicht in der Cloud hinzugefügt werden.
1. Stellen Sie sicher, dass noch kein anderer Benutzer oder Kontakt den Benutzernamen aufweist, den Sie dem neuen Benutzer zuweisen möchten. Benutzernamen müssen in Azure AD eindeutig sein.
1. Weitere Informationen für Ihr Azure AD finden Sie unter [Azure AD-Rollen und -Administratoren](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators).
1. Informieren Sie sich über die [Domänennamen,](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) für Ihr Azure AD.
1. Überprüfen Sie die [Überwachungsprotokolle](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators), um detailliertere Informationen zu einem kürzlich erstellten oder gelöschten Benutzer zu erhalten, z. B. wer die Aktion ausgeführt hat und wann.
1. Weitere Informationen zum Hinzufügen neuer Benutzer finden Sie unter [Verwenden des Azure-Portals zum Erstellen eines neuen Benutzers in Azure AD.](/azure/active-directory/active-directory-users-create-azure-portal)
1. [Azure AD-Administratorrollen:](/azure/active-directory/active-directory-assign-admin-roles)Administratorrollenberechtigungen in Azure Active Directory
1. Sie können [auch Azure AD PowerShell verwenden, um einen neuen Benutzer zu erstellen.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
