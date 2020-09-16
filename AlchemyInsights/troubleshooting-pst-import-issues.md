---
title: Behandlung von Problemen beim PST-Import
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 5fdb713f321e5c9f67a6078739c31a90571b913d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757739"
---
# <a name="troubleshooting-pst-import-issues"></a>Behandlung von Problemen beim PST-Import

- Wenn Sie innerhalb des Outlook-Clients importieren, lesen Sie [Beheben von Problemen beim Importieren einer PST-Datei in Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Wenn Sie den Importdienst verwenden und er hängen bleibt, beachten Sie bitte, dass jede in den Azure-Speicherort hochgeladene PST-Datei nicht größer als 20 GB sein sollte. PST-Dateien mit mehr als 20 GB können sich auf die Leistung des PST-Importprozesses auswirken.

- Wenn Sie den Status eines bestimmten Importauftrags überprüfen möchten, können Sie [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest) verwenden.

- Ausführliche Informationen zum Importdienst finden Sie unter [Übersicht über das Importieren der PST-Dateien Ihrer Organisation](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
