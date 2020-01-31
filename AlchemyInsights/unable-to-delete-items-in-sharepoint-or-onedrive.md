---
title: Elemente in SharePoint oder OneDrive können nicht gelöscht werden.
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571253"
---
# <a name="unable-to-delete-items"></a>Elemente können nicht gelöscht werden

Aufbewahrungsrichtlinien können dazu führen, dass Sie die entsprechenden Haltestatus, die dieses Problem verursachen, entweder deaktivieren oder ausschließen müssen. Nach dem Entfernen einer Aufbewahrungsrichtlinie oder eines Haltestatus kann es bis zu 24 Stunden dauern, bis die Änderung wirksam wird. Stellen Sie sicher, dass kein [Aufbewahrungsrichtlinien](https://docs.microsoft.com/office365/securitycompliance/retention-policies) Setup für das Element vorhanden ist.

Die Website hat möglicherweise die Speichergrenzwerte überschritten, das [Websitekontingent](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) erhöht und das Element gelöscht.

Stellen Sie sicher, dass das Element nicht für einen anderen Benutzer [ausgecheckt](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) ist.

Schließlich können Administratoren [SharePoint-Muster und-Methoden](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) verwenden, das eine Bibliothek mit PowerShell-Befehlen enthält, mit denen Sie komplexe Verwaltungsaktionen wie das Löschen hartnäckiger Elemente erzwingen können.
- [PNP-Datei entfernen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP-Ordner entfernen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP-Listenelement entfernen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP-Liste entfernen](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP-Feld entfernen (Spalte)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)