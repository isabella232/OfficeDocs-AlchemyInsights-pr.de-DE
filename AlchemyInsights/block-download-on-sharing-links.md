---
title: Blockieren des Downloads für Freigabelinks
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
- "9000213"
- "5715"
ms.openlocfilehash: 5837013a71648d5d53cd215c3e3489f3de5528d5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685741"
---
# <a name="block-download-on-sharing-links"></a>Blockieren des Downloads für Freigabelinks

**Download blockieren** ist für **schreibgeschützte Links** zu Office-Dokumenten verfügbar. Wenn Sie diese Option auswählen, werden Personen, die über den von Ihnen erstellten Link Zugriff auf die Datei erhalten, keine Optionen zum Herunterladen, Drucken oder Kopieren der Datei angezeigt.

Administratoren können über die `BlockDownloadLinksFileType`-Einstellung in den PowerShell-Cmdlets [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) oder [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) steuern, ob die Einstellung "Download blockieren" nur für Office-Dateien angezeigt wird oder nicht.
