---
title: DLP-Regel für SSN nicht funktionsfähig
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: d2d21fb5546d36990d69b76e3ceb72ce2edf3d80
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29933479"
---
Haben Sie Probleme mit der **Data Loss Prevention (DLP)** für Inhalte mit einer **Sozialversicherungsnummer (SSN)** , wenn ein anderes vertrauliche Informationen in Office 365 verwenden nicht ordnungsgemäß ausgeführt? Wenn dies der Fall ist, stellen Sie sicher, dass Ihre Inhalte enthält die erforderliche Informationen für die DLP-Richtlinie suchen. 
  
Beispiel für eine SSN-Richtlinie mit einer Vertrauensstufe von 85 % konfiguriert, die folgenden ausgewertet werden und müssen erkannt werden, für die Regel ausgelöst:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 Ziffern, die in einem Muster formatierte oder unformatierte sein können 
    
- **[Muster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Vier Funktionen suchen SSNs in vier verschiedene Muster: 
    
  - Func_ssn sucht nach US-Sozialversicherungsnummern von vor 2011, die mithilfe von Bindestrichen oder Leerzeichen (ddd-dd-dddd ODER ddd dd dddd) formatiert sind 
    
  - Func_unformatted_ssn sucht nach US-Sozialversicherungnummern von vor 2011, die als neun aufeinander folgende Ziffern (ddddddddd) formatiert sind
    
  - Func_randomized_formatted_ssn sucht nach US-Sozialversicherungsnummern von nach 2011, die mithilfe von Bindestrichen oder Leerzeichen (ddd-dd-dddd ODER ddd dd dddd) formatiert sind 
    
  - Func_randomized_unformatted_ssn sucht nach US-Sozialversicherungnummern von nach 2011, die als neun aufeinander folgende Ziffern (ddddddddd) formatiert sind
    
- **[Prüfsumme:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nein, keine Prüfsumme vorhanden ist 
    
- **[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Eine DLP-Richtlinie ist 85 % sicher, dass diese Art von vertraulichen Informationen festgestellt wurde "If"; innerhalb einer Nähe von 300 Zeichen: 
    
  - Die [Funktion Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) sucht nach Inhalten, die dem Muster entspricht. 
    
  - Ein Schlüsselwort aus [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) gefunden wird. Enthält Beispiele für Schlüsselwörter: *soziale Sicherheit, Sozialleistungen #, Krankenversicherung, SSN* . Beispielsweise würde im folgende Beispiel für die SSN DLP-Richtlinie ausgelöst: **SSN: 489-36-8350**
    
Weitere Informationen zu Anforderungen für SSNs für Ihre Inhalte erkannt werden, finden Sie im folgenden Abschnitt in diesem Artikel: [Was der vertraulichen Informationstypen SSNs suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Mit einer anderen integrierten vertrauliche Informationstyp finden Sie Informationen im folgenden Artikel auf was für andere Typen erforderlich ist: [was der vertraulichen Informationstypen suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

