---
title: Leistungsprobleme – SharePoint oder OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068400"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint oder OneDrive langsam, unzugänglich oder nicht verfügbar für mehrere Benutzer

SharePoint oder OneDrive ist möglicherweise langsam, unzugänglich oder nicht verfügbar oder kann Dienst nicht verfügbar oder 503-Fehler aus mehreren Gründen anzeigen:
  
- Wenn Ihre SharePoint-oder OneDrive-Website für mehrere Benutzer langsam oder verzögert ist, gibt es möglicherweise ein vorübergehendes Dienst Problem, bei dem Benutzer bei Zugriff auf SharePoint-Websites oder OneDrive-Inhalte zeitweilig Verzögerungen oder Navigationsfehler auftreten. Überprüfen Sie das [Dienststatus-Dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , um zu sehen, ob Ihre Organisation betroffen ist.
  
- Bei dem Versuch, zu SharePoint-oder OneDrive-Websites zu navigieren, erhalten Benutzer möglicherweise einen Fehler " *503 Server ist ausgelastet* ". Dieser Fehler kann durch Drosselung im SharePoint-Dienst verursacht werden. SharePoint Online verwendet Einschränkung, um eine optimale Leistung und Zuverlässigkeit des Diensts SharePoint Online verwalten. Einschränkungsgrenzwerte Ruft die Anzahl von Aktionen eines Benutzers oder gleichzeitige (von Code- oder Skriptblock), um Ressourcen zu verhindern. Weitere Informationen zur Drosselung finden Sie unter vermeiden Sie eine [Drosselung oder Blockierung in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Wenn Sie eine langsame Leistung mit einer **klassischen** oder **modernen** SharePoint-Website oder-Seite erleben, verwenden Sie das Seiten [Diagnosetool](https://aka.ms/perftool) , um die Seiten zu analysieren.
  
- Wenn Sie weiterhin eine allgemeine langsame Leistung erzielen, lesen Sie die Ressourcen unten in diesem Artikel: [Einführung in die Leistungsoptimierung für SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  