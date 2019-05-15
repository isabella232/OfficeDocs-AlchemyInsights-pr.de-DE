---
title: Elemente in SharePoint oder OneDrive können nicht gelöscht werden.
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057712"
---
# <a name="unable-to-delete-items"></a>Elemente können nicht gelöscht werden

Haben Sie Probleme beim Löschen von Elementen?

- Stellen Sie immer sicher, dass Sie über die [entsprechenden Berechtigungen](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) zum Löschen des Elements verfügen, oder wenn der [Websitesammlungsadministrator](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) versucht, das Element zu entfernen.

- Stellen Sie sicher, dass keine [Aufbewahrungsrichtlinie](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) für das Element vorhanden ist.

- Stellen Sie sicher, dass das Element nicht an einen anderen Benutzer [ausgecheckt](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) ist.

- Schließlich können Administratoren [SharePoint Patterns and Practices](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) verwenden, die eine Bibliothek mit PowerShell-Befehlen enthalten, mit denen Sie komplexe Verwaltungsaktionen wie das Erzwingen des Löschens von hartnäckigen Elementen ausführen. 
- [PNP-Datei entfernen](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP-Ordner entfernen](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP-Listenelement entfernen](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP-Liste entfernen](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP-Feld entfernen (Spalte)](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)