---
title: Problembehandlung bei Zugriff verweigerten Nachrichten an OneDrive für Unternehmen Websites
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692800"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Problembehandlung bei Zugriff verweigerten Nachrichten an OneDrive für Unternehmen Websites

Dieses Problem tritt am häufigsten auf, wenn ein Benutzer gelöscht und mit demselben Benutzerprinzipalnamen (User Principal Name, UPN) neu erstellt wird. Das neue Konto wird mithilfe eines anderen Werts für PUID (Passport Unique ID) erstellt. Wenn der Benutzer versucht, auf eine Websitesammlung oder deren OneDrive zuzugreifen, verfügt der Benutzer über eine falsche PUID. Ein zweites Szenario umfasst die Verzeichnissynchronisierung mit einer Active Directory Organisationseinheit (Organizational Unit, OU). Wenn sich Benutzer bereits bei SharePoint angemeldet haben und dann in eine andere Organisationseinheit verschoben und mit SharePoint erneut synchronisiert wurden, kann dieses Problem auftreten.

1. Um dieses Problem zu beheben, sollten Sie den ursprünglichen UPN mit den Schritten in diesem Artikel wiederherstellen, um [einen Benutzer in Microsoft 365 wiederherzustellen](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Wenn Sie den ursprünglichen Benutzer nicht wiederherstellen können, sollten Sie den alten Benutzer aus der OneDrive-Website mithilfe dieser Schritte entfernen, indem Sie [einen Benutzer aus der Liste Benutzerinformationen entfernen](). 
3. Nachdem Sie dies abgeschlossen haben, können Sie überprüfen, ob der Benutzer Administratorrechte für die OneDrive-Website hat, indem Sie die Schritte zum [Hinzufügen von Administratoren für die OneDrive eines Benutzers](https://docs.microsoft.com/sharepoint/manage-user-profiles) ausführen.

Weitere Informationen zu Berechtigungsstufen finden Sie im Artikel [Grundlegendes zu Berechtigungsstufen in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
