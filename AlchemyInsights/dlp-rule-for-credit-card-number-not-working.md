---
title: DLP-Regel für Kreditkartennummer nicht funktionsfähig
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: a56f32b54e6cb32fa044d26d08868bac8c368de5
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29470501"
---
Haben Sie Probleme mit der **Data Loss Prevention (DLP)** funktioniert nicht für Inhalt mit einer **Kreditkartennummer** , wenn ein anderes DLP vertrauliche Informationen in Office 365 verwenden? Wenn dies der Fall ist, stellen Sie sicher, Ihre Inhalte enthält die erforderliche Informationen zum Auslösen der DLP-Richtlinie, wenn sie ausgewertet wird. Beispiel für eine **Kreditkarte Richtlinie** mit einer Vertrauensstufe von 85 % konfiguriert, die folgenden ausgewertet werden und erkannt werden muss, für die Regel ausgelöst: 
  
- **[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 Stellen die formatiert werden können oder unformatierte (Dddddddddddddddd), und geben Sie den Test mit Luhn müssen. 
    
- **[Muster:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Sehr komplex und robuste Muster, das Karten aus alle wichtigen Marken weltweit, einschließlich Visa, Mastercard, Discover-Karte, JCB, amerikanische Express, Geschenkgutscheine und Bestellung Karten erkennt. 
    
- **[Prüfsumme:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, die Prüfsumme Luhn 
    
- **[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Eine DLP-Richtlinie ist 85 % sicher, dass diese Art von vertraulichen Informationen festgestellt wurde "If"; innerhalb einer Nähe von 300 Zeichen: 
    
  - Die Funktion Func_credit_card findet Inhalte, die dem Muster entsprechen.
    
  - Eine der folgenden Bedingungen trifft zu: 
    
  - Ein Schlüsselwort aus Keyword_cc_verification wurde gefunden.
    
  - Ein Schlüsselwort aus Keyword_cc_name wurde gefunden.
    
  - Die Funktion Func_expiration_date findet ein Datum im richtigen Datumsformat.
    
  - Die Prüfsumme stimmt.
    
    Beispielsweise würde im folgende Beispiel für eine DLP Kreditkarte Anzahl Richtlinie ausgelöst:
    
  - Visa: 4485 3647 3952 7352 
    
  - Gültig bis: 2/2009
    
Weitere Informationen zu Anforderungen für eine **Kreditkartennummer** für Ihre Inhalte erkannt werden, finden Sie im folgenden Abschnitt in diesem Artikel: [Was der vertraulichen Informationstypen für Kreditkarte-suchen](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Mit einer anderen integrierten vertrauliche Informationstyp finden Sie Informationen im folgenden Artikel auf was für andere Typen erforderlich ist: [was der vertraulichen Informationstypen suchen](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

