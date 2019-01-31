---
title: DLP-Regel für US / Großbritannien Reisepassnummer nicht funktionsfähig
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 5722f7b6c9a2f905fed2ef4164787e020260edf7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656422"
---
Haben Sie Probleme mit **Data Loss Prevention (DLP)** funktioniert nicht für Inhalt mit einer **US / Großbritannien Reisepassnummer** bei Verwendung eines DLP-Typs vertraulicher Informationen in Office 365? In diesem Fall enthält stellen Sie sicher, dass Ihre Inhalte die erforderliche Informationen für welche die DLP-Richtlinie Ansichtsseite sucht bei der Auswertung. 
  
Beispiel für eine **US / Großbritannien Reisepassnummer** mit einer Vertrauensstufe von 75 % konfigurierte Richtlinie, die folgenden ausgewertet werden und muss für die Regel ausgelöst erkannt werden 
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Neun Ziffern 
    
- **[Muster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Neun aufeinander folgenden Ziffern 
    
- **[Prüfsumme:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nein, keine Prüfsumme vorhanden ist 
    
- **[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Eine DLP-Richtlinie ist 75 % sicher, dass diese Art von vertraulichen Informationen festgestellt wurde "If"; innerhalb einer Nähe von 300 Zeichen: 
    
  - Die Funktion Func_usa_uk_passport findet Inhalte, die dem Muster entsprechen.
    
  - Ein Schlüsselwort aus Keyword_passport wurde gefunden.
    
    Im folgende Beispiel würden beispielsweise trigger für die **US / Großbritannien Reisepassnummer** Richtlinie: US Reisepassnummer 123456789 
    
Weitere Informationen zu für eine US Anforderungen / Großbritannien Reisepassnummer für Ihre Inhalte erkannt werden, finden Sie unter den folgenden Abschnitt in diesem Artikel: [was der vertraulichen Informationstypen Darstellung für US / Großbritannien Reisepassnummer](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Mit einer anderen integrierten vertrauliche Informationstyp finden Sie Informationen im folgenden Artikel auf was für andere Typen erforderlich ist: [was der vertraulichen Informationstypen suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

