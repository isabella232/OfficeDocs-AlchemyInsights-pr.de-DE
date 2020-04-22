---
title: DLP benötigt möglicherweise einen benutzerdefinierten Typ
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: b83bb77383e2ae7e78c31f35c972182c54487c60
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704488"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP benötigt möglicherweise einen benutzerdefinierten Typ

**Wichtig**: Während dieser beispiellosen Zeiten unternehmen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online und OneDrive-Dienste weiterhin in hohem Ausmaß verfügbar bleiben – Bitte besuchen Sie [SharePoint Online – Temporäre Feature-Anpassungen](https://aka.ms/ODSPAdjustments), um weitere Informationen zu erhalten.

**DLP erfordert möglicherweise einen benutzerdefinierten Informationstyp.**

Mit einer Richtlinie zur Verhinderung von Datenverlust (Data Loss Prevention, DLP) können Sie vertrauliche Daten in Ihrer Organisation identifizieren und schützen. In einigen Szenarien müssen Sie möglicherweise einen eigenen **benutzerdefinierten** Typ für vertrauliche Informationen erstellen, um die Daten Ihrer Organisation zu schützen.

Beispielsweise kann es sein, dass Ihre Organisation Mitarbeiter-IDs oder andere Daten in einem bestimmten für Ihre org spezifischen Format identifizieren und schützen muss. Wenn dies der Fall ist, finden Sie weitere Informationen in den folgenden Artikeln.
  
 **Anpassen eines benutzerdefinierten vertraulichen Informationstyps**
  
Wenn ein integrierter vertraulicher Informationstyp Ihren Anforderungen mit nur wenigen Optimierungen entspricht, können Sie [einen integrierten vertraulichen Informationstyp anpassen](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type). Beispielsweise können Sie Stichwörter hinzufügen oder entfernen oder unterstützende Beweise wie ein Datum oder eine Adresse hinzufügen oder entfernen.
  
 **Erstellen eines benutzerdefinierten vertraulichen Informationstyps**
  
Wenn Sie jedoch einen anderen Typ vertraulicher Informationen insgesamt identifizieren und schützen müssen, können Sie [einen benutzerdefinierten Typ vertraulicher Informationen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) auf der Benutzeroberfläche des Security & Compliance Center erstellen.
  
**Erstellen eines benutzerdefinierten Typs für vertrauliche Informationen in Security & Compliance Center PowerShell**

Wenn die Benutzeroberfläche nicht alle benötigten Optionen bereitstellt, können Sie [in Security & Compliance Center PowerShell einen benutzerdefinierten Typ für vertrauliche Informationen erstellen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell). Wenn Sie mit einer XML-Datei beginnen, können Sie jede verfügbare Option verwenden.
