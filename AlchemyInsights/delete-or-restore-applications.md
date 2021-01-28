---
title: Löschen oder Wiederherstellen von Anwendungen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013957"
---
# <a name="delete-or-restore-applications"></a>Löschen oder Wiederherstellen von Anwendungen

**So löschen Sie eine Anwendung aus Ihrem Azure AD-Mandanten:**

1. Wählen Sie **im Azure AD-Portal** **Enterprise-Anwendungen aus.** Suchen Und wählen Sie dann die Anwendung aus, die Sie löschen möchten.
2. Wählen Sie **im Abschnitt "Verwalten"** im linken Bereich **"Eigenschaften" aus.**
3. Wählen **Sie "Löschen"** und dann **"Ja"** aus, um zu bestätigen, dass Sie die App aus Ihrem Azure AD-Mandanten löschen möchten.

Weitere Informationen zum Löschen einer App finden Sie unter Schnellstart: Löschen einer Anwendung aus Ihrem [Azure Active Directory (Azure AD)-Mandanten.](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

In PowerShell entfernt das [Cmdlet "Remove-AzureADApplicationProxyApplication" Anwendungsproxykonfigurationen](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) aus einer bestimmten Anwendung in Azure Active Directory und kann die Anwendung vollständig löschen, falls angegeben.

Sie können **eine gelöschte Anwendung mithilfe** von PowerShell wiederherstellen. Nachdem die wiederherzustellende Anwendung identifiziert wurde, können Sie sie mithilfe von [Restore-AzureADDeletedApplication wiederherstellen.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
