---
title: DLP-Regel für uns Bankkontonummer nicht funktionsfähig
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 9ebfa6bc09cef9ab7c30bddb4fcb8b6be3ab55a5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916415"
---
Haben Sie Probleme mit der **Data Loss Prevention (DLP)** funktioniert nicht für Inhalt mit einer **Kontonummer US** , wenn ein anderes DLP vertrauliche Informationen in Office 365 verwenden? In diesem Fall enthält stellen Sie sicher, dass Ihre Inhalte die erforderliche Informationen für welche die DLP-Richtlinie Ansichtsseite sucht bei der Auswertung. 
  
Beispiel für eine **Kontonummer US** -Richtlinie mit einer Vertrauensstufe von 85 % konfiguriert, die folgenden ausgewertet werden und müssen erkannt werden, für die Regel ausgelöst: 
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8 bis 17 Ziffern 
    
- **[Muster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8 bis 17 aufeinander folgenden Ziffern. 
    
- **[Prüfsumme:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nein, keine Prüfsumme vorhanden ist 
    
- **[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Eine DLP-Richtlinie ist 75 % sicher, dass diese Art von vertraulichen Informationen festgestellt wurde "If"; innerhalb einer Nähe von 300 Zeichen: 
    
  - Der reguläre Ausdruck Regex_usa_bank_account_number sucht nach Inhalten, die dem Muster entspricht
    
  - Ein Schlüsselwort aus Keyword_usa_Bank_Account wurde gefunden.
    
    Beispielsweise würde im folgende Beispiel für die **USA Bankkontonummer** Richtlinie ausgelöst: Bankkonto 78344011 
    
Weitere Informationen zu Anforderungen für eine **Kontonummer US** für Ihre Inhalte erkannt werden, finden Sie im folgenden Abschnitt in diesem Artikel: [Was der vertraulichen Informationstypen US Bankkontonummer suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Mit einer anderen integrierten vertrauliche Informationstyp finden Sie Informationen im folgenden Artikel auf was für andere Typen erforderlich ist: [was der vertraulichen Informationstypen suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

