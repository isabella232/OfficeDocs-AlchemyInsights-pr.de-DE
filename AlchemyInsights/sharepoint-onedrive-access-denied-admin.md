---
title: Behandeln von Zugriffs verweigerten Nachrichten
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707953"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Behandeln von Zugriffs verweigerten Nachrichten in Sharepoint/OneDrive Admin Center

Wenn Sie beim Versuch, zu einem Sharepoint/OneDrive Admin Center zu navigieren, eine Nachricht mit dem Zugriff verweigert erhalten, stellen Sie sicher, dass Sie dem Benutzer eine [Lizenz zuweisen.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Wenn der Benutzer über eine Lizenz verfügt, sollten Sie auch sicherstellen, dass ihm eine Administratorrolle zugewiesen ist, [die](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) auf die Admin Center zugreifen kann.

Dieses Problem kann auch auftreten, wenn ein Benutzer gelöscht und mit demselben Benutzerprinzipalnamen (User Principal Name, UPN) neu erstellt wird. Das neue Konto wird mithilfe eines anderen PUID -Werts (Passport Unique ID) erstellt. Wenn der Benutzer versucht, auf eine Websitesammlung oder sein OneDrive zu zugreifen, hat der Benutzer eine falsche PUID. Ein zweites Szenario umfasst die Verzeichnissynchronisierung mit einer Active Directory-Organisationseinheit (Ou). Wenn benutzer sich bereits bei SharePoint angemeldet haben und dann in eine andere Organisationseinheit verschoben und mit SharePoint neu synchronisiert werden, kann dieses Problem auf sie bzw. die Benutzer bzw. die Benutzerin sharePoint angewendet werden.

Um dieses Problem zu beheben, sollten Sie den ursprünglichen UPN mit den Schritten im Artikel Wiederherstellen eines Benutzers [in Microsoft 365 wiederherstellen.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

Hinweis: Wenn ein OneDrive- oder SharePoint Admin Center nicht für mehrere Benutzer verfügbar ist, die zuvor Zugriff hatten, kann ein temporäres Dienstproblem vorliegen.  [Überprüfen Sie das Dienstintegashboard](https://portal.office.com/adminportal/home#/servicehealth).


