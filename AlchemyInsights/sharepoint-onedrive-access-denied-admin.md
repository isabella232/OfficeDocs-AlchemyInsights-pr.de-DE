---
title: Problembehandlung bei Zugriff verweigerten Nachrichten
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503527"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Problembehandlung bei Zugriff verweigerten Nachrichten in SharePoint/OneDrive Admin Center

Wenn Sie eine Meldung zum Zugriff verweigert erhalten, wenn Sie versuchen, zu einem SharePoint/OneDrive Admin Center zu navigieren, stellen Sie sicher, dass Sie [dem Benutzer eine Lizenz zuweisen](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Wenn der Benutzer über eine Lizenz verfügt, sollten Sie auch sicherstellen, dass ihm [eine Administratorrolle zugewiesen](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) ist, die auf die Admin Center zugreifen kann.

Dieses Problem kann auch auftreten, wenn ein Benutzer gelöscht und mit demselben Benutzerprinzipalnamen (User Principal Name, UPN) neu erstellt wird. Das neue Konto wird mithilfe eines anderen Werts für PUID (Passport Unique ID) erstellt. Wenn der Benutzer versucht, auf eine Websitesammlung oder deren OneDrive zuzugreifen, verfügt der Benutzer über eine falsche PUID. Ein zweites Szenario umfasst die Verzeichnissynchronisierung mit einer Active Directory Organisationseinheit (Organizational Unit, OU). Wenn sich Benutzer bereits bei SharePoint angemeldet haben und dann in eine andere Organisationseinheit verschoben und mit SharePoint erneut synchronisiert wurden, kann dieses Problem auftreten.

Um dieses Problem zu beheben, sollten Sie den ursprünglichen UPN mit den Schritten im Artikel wiederherstellen, [einen Benutzer in Office 365 wiederherstellen](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Hinweis: Wenn ein OneDrive-oder SharePoint Admin Center nicht für mehrere Benutzer verfügbar ist, die zuvor Zugriff hatten, ist möglicherweise ein vorübergehendes Dienst Problem aufgetreten.  [Überprüfen Sie das Dienst Integritäts Dashboard](https://portal.office.com/adminportal/home#/servicehealth).


