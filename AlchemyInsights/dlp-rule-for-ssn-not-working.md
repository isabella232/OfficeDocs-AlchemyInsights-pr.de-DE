---
title: DLP-Regel für SSN funktioniert nicht
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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404416"
---
Haben Sie Probleme mit **Data Loss Prevention (DLP)** , die nicht für Inhalte, die eine Sozialversicherungs **Nummer (SSN)** enthalten, bei Verwendung eines vertraulichen informationstyps in Office 365? Wenn dies der Fall ist, stellen Sie sicher, dass Ihre Inhalte die erforderlichen Informationen für die Suche nach der DLP-Richtlinie enthalten. 
  
Bei einer SSN-Richtlinie, die mit einem Konfidenzniveau von 85% konfiguriert wurde, werden beispielsweise die folgenden Werte ausgewertet und müssen erkannt werden, damit die Regel ausgelöst wird:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 Ziffern, die sich möglicherweise in einem formatierten oder unformatierten Muster befinden 
    
- **[Muster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Vier Funktionen suchen nach SSNs in vier verschiedenen Mustern: 
    
  - Func_ssn findet SSNs mit einer starken Formatierung vor 2011, die mit Bindestrichen oder Leerzeichen (DDD-DD-dddd oder DDD DD dddd) formatiert sind.
    
  - Func_unformatted_ssn findet SSNs mit einer starken Formatierung vor 2011, die unformatiert sind, als neun aufeinanderfolgende Ziffern (ddddddddd)
    
  - Func_randomized_formatted_ssn findet Post-2011 SSNs, die mit Bindestrichen oder Leerzeichen (DDD-DD-dddd oder DDD DD dddd) formatiert sind.
    
  - Func_randomized_unformatted_ssn findet Post-2011 SSNs, die unformatiert sind, als neun aufeinanderfolgende Ziffern (ddddddddd)
    
- **[Prüfsumme:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nein, es gibt keine prüfSumme 
    
- **[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Eine DLP-Richtlinie ist 85% sicher, dass Sie diese Art von vertraulichen Informationen erkannt hat, wenn Sie innerhalb einer Nähe von 300 Zeichen: 
    
  - Die [Funktion Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) sucht nach Inhalten, die mit dem Muster übereinstimmen. 
    
  - Ein Schlüsselwort aus [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) wurde gefunden. Beispiele für Stichwörter: *soziale Sicherheit, soziale Sicherheit, Soc Sec, SSN* . Das folgende Beispiel würde beispielsweise für die DLP-SSN-Richtlinie auslösen: **SSN: 489-36-8350**
    
Weitere Informationen dazu, was für die Erkennung von SSNs für Ihre Inhalte erforderlich ist, finden Sie im folgenden Abschnitt in diesem Artikel: [was die Typen vertraulichEr Informationen für SSNs suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Verwenden Sie einen anderen integrierten vertraulichen Informationstyp, um Informationen darüber zu erhalten, was für andere Typen erforderlich ist: [was die Typen für vertrauliche Informationen suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

