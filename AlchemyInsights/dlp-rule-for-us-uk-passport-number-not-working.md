---
title: DLP-Regel für US/UK Passport-Nummer nicht funktionsfähig
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bb80ef07364a575f6032bb105cff83cd8f95bd63
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404380"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Probleme mit DLP-US/UK-Passport-Nummern

Haben Sie Probleme mit dem **Schutz vor Datenverlust (DLP)** , die für Inhalte, die eine **US/UK-Passport-Nummer** enthalten, nicht arbeiten, wenn Sie einen DLP-vertraulichen Informationstyp in O365 verwenden? Wenn dies der Fall ist, stellen Sie sicher, dass Ihre Inhalte die erforderlichen Informationen für die Anforderungen der DLP-Richtlinie bei der Auswertung enthalten. 
  
Für eine **US/UK Passport Number** -Richtlinie, die mit einem Konfidenzniveau von 75% konfiguriert wurde, werden beispielsweise die folgenden Werte ausgewertet und müssen erkannt werden, damit die Regel ausgelöst wird. 
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Neun Ziffern 
    
- **[Muster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Neun aufeinanderfolgende Ziffern 
    
- **[Prüfsumme:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nein, es gibt keine prüfSumme 
    
- **[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Eine DLP-Richtlinie ist 75% sicher, dass Sie diese Art von vertraulichen Informationen erkannt hat, wenn Sie innerhalb einer Nähe von 300 Zeichen: 
    
  - Die Funktion Func_usa_uk_passport findet Inhalte, die dem Muster entsprechen.
    
  - Ein Schlüsselwort aus Keyword_passport wurde gefunden.
    
    Das folgende Beispiel würde beispielsweise für die **US/UK Passport Number-** Richtlinie auslösen: U.S. passport Number 123456789 
    
Weitere Informationen dazu, was erforderlich ist, damit eine US/UK-Passport-Nummer für Ihre Inhalte erkannt wird, finden Sie im folgenden Abschnitt dieses Artikels: [was die vertraulichEn Informationstypen für die US/UK Passport-Nummer suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Verwenden Sie einen anderen integrierten vertraulichen Informationstyp, um Informationen darüber zu erhalten, was für andere Typen erforderlich ist: [was die Typen für vertrauliche Informationen suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

