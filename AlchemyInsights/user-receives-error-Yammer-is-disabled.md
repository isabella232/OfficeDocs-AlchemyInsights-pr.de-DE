---
title: 'Benutzer erhält den Fehler: AADSTS7000112 Yammer ist deaktiviert'
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: 3a3a1b531f3d775f7e5150ce86733a3012df8d0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47796647"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Benutzer erhält den Fehler: AADSTS7000112 Yammer ist deaktiviert

Wenn die Fehlermeldung "AADSTS7000112: Anwendung '00000005-0000-0ff1-ce00-000000000000' (Yammer) ist deaktiviert" angezeigt wird, liegt ein Problem mit dem Dienstprinzipal in Azure AD vor. Möglicherweise hat ein Administrator den Dienstprinzipal deaktiviert, um den Zugriff auf Yammer zu blockieren.

Das Deaktivieren des Dienstprinzipals wird nicht empfohlen und kann zu weiteren Problemen führen. Weitere Informationen zum unterstützten Ansatz für dass Blockieren des Benutzerzugriffs auf Yammer finden Sie unter [Deaktivieren des Zugriffs auf Yammer für Microsoft 365-Benutzer](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

So beheben Sie dieses Problem im Azure-Portal und stellen den Benutzerzugriffs auf Yammer wieder her

1.  Öffnen Sie die Azure Active Directory-Seite, und wählen Sie im linken Navigationsbereich **Enterprise-Anwendungen** unter **Verwalten** aus.
3.  Geben Sie **Office 365 Yammer** in das Suchfeld ein, und wählen Sie den Namen der Anwendung aus, um die Einstellungen zu öffnen.
4.  Wählen Sie im linken Navigationsbereich unter **Eigenschaften****Verwalten** aus.
5.  Legen Sie den Wert für **Für Benutzeranmeldung aktiviert?** auf **Ja** fest, und wählen Sie dann **Speichern** aus.
6.  Melden Sie sich wieder bei Yammer an. Möglicherweise müssen Sie Cookies löschen.

Alternativ können Sie den Wert unter Verwendung von PowerShell-Befehlen festlegen. Weitere Informationen finden Sie unter [Fehler "Leider können wir Sie nicht anmelden" beim Klicken auf die Yammer-Kachel in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 