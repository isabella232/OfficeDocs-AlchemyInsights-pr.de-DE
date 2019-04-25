---
title: DLP-Regel für Kreditkartennummer nicht funktionsfähig
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404493"
---
Haben Sie Probleme mit **Data Loss Prevention (DLP)** , die nicht für Inhalte, die eine **Kreditkartennummer** enthalten, bei Verwendung eines DLP-vertraulichen Informationstyps in O365? Wenn dies der Fall ist, stellen Sie sicher, dass Ihre Inhalte die erforderlichen Informationen enthalten, um die DLP-Richtlinie auszulösen, wenn Sie ausgewertet wird. Bei einer **Kreditkarten Richtlinie** , die mit einem Konfidenzniveau von 85% konfiguriert wurde, werden beispielsweise folgende Werte ausgewertet und müssen erkannt werden, damit die Regel ausgelöst wird: 
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 Ziffern, die formatiert oder unformatiert (dddddddddddddddd) werden können und den Luhn-Test bestehen müssen. 
    
- **[Muster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Sehr komplexes und robustes Muster, das Karten aller wichtigen Marken weltweit erkennt, einschließlich Visa, MasterCard, Discover Card, JCB, American Express, Geschenkkarten und dinerkarten. 
    
- **[Prüfsumme:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, die Luhn-Prüfsumme 
    
- **[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Eine DLP-Richtlinie ist 85% sicher, dass Sie diese Art von vertraulichen Informationen erkannt hat, wenn Sie innerhalb einer Nähe von 300 Zeichen: 
    
  - Die Funktion Func_credit_card findet Inhalte, die dem Muster entsprechen.
    
  - Eine der folgenden Bedingungen trifft zu: 
    
  - Ein Schlüsselwort aus Keyword_cc_verification wurde gefunden.
    
  - Ein Schlüsselwort aus Keyword_cc_name wurde gefunden.
    
  - Die Funktion Func_expiration_date findet ein Datum im richtigen Datumsformat.
    
  - Die Prüfsumme wird übergeben.
    
    Das folgende Beispiel würde beispielsweise für eine DLP-Kreditkartennummern Richtlinie auslösen:
    
  - Visa: 4485 3647 3952 7352 
    
  - Expires: 2/2009
    
Weitere Informationen dazu, was erforderlich ist, damit eine **Kreditkartennummer** für Ihre Inhalte erkannt wird, finden Sie im folgenden Abschnitt dieses Artikels: [was die Typen vertraulicher Informationen für Kreditkartennummern suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Verwenden Sie einen anderen integrierten vertraulichen Informationstyp, um Informationen darüber zu erhalten, was für andere Typen erforderlich ist: [was die Typen für vertrauliche Informationen suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

