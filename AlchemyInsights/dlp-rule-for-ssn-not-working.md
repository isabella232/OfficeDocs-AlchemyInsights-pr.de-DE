---
title: DLP-Regel für SSN nicht funktionsfähig
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: fffd355279b064b31c0a8bf60518b15ee1ed1848
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389432"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP-Probleme mit Sozialversicherungsnummern

Haben Sie Probleme mit der Verhinderung von **Datenverlust (DLP)** , die bei der Verwendung eines vertraulichen Informationstyps in Office 365 nicht für Inhalte mit einer Sozialversicherungs **Nummer (SSN)** funktioniert? Wenn dies der Fall ist, stellen Sie sicher, dass Ihre Inhalte die erforderlichen Informationen für die Suchfunktion der DLP-Richtlinie enthalten. 
  
Für eine SSN-Richtlinie, die mit einer Konfidenz Stufe von 85% konfiguriert ist, werden beispielsweise die folgenden Werte ausgewertet und müssen erkannt werden, damit die Regel ausgelöst wird:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 Ziffern, die sich möglicherweise in einem formatierten oder unformatierten Muster befinden

- **[Muster:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Vier Funktionen suchen nach Sozialversicherungsnummern in vier verschiedenen Mustern:

  - Func_ssn findet Sozialversicherungsnummern mit starker Formatierung vor 2011, die mit Bindestrichen oder Leerzeichen formatiert sind (DDD-DD-dddd oder DDD DD dddd)

  - Func_unformatted_ssn findet Sozialversicherungsnummern mit starker Formatierung vor 2011, die als neun aufeinanderfolgende Ziffern (ddddddddd) unformatiert sind.

  - Func_randomized_formatted_ssn findet Post-2011-Sozialversicherungsnummern, die mit Bindestrichen oder Leerzeichen formatiert sind (DDD-DD-dddd oder DDD DD dddd)

  - Func_randomized_unformatted_ssn findet Post-2011-Sozialversicherungsnummern, die als neun aufeinanderfolgende Ziffern (ddddddddd) unformatiert sind.

- **[Prüfsumme:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nein, es gibt keine Prüfsumme

- **[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Eine DLP-Richtlinie ist 85% sicher, dass diese Art von vertraulichen Informationen erkannt wurde, wenn Sie in einer Nähe von 300 Zeichen:

  - Die [Funktion Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) findet Inhalte, die mit dem Muster übereinstimmen.

  - Ein Schlüsselwort aus [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) wurde gefunden. Beispiele für Schlüsselwörter: *soziale Sicherheit, soziale Sicherheit #, Soc Sec, SSN* . Das folgende Beispiel würde beispielsweise für die DLP-SSN-Richtlinie ausgelöst: **SSN: 489-36-8350**
  
Weitere Informationen dazu, was für die Sozialversicherungsnummern-Erkennung für Ihre Inhalte erforderlich ist, finden Sie im folgenden Abschnitt in diesem Artikel: [was die Typen für vertrauliche Informationen für Sozialversicherungsnummern suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Unter Verwendung eines anderen integrierten vertraulichen Informationstyps finden Sie im folgenden Artikel Informationen darüber, was für andere Typen erforderlich ist: [was die Typen für vertrauliche Informationen suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  