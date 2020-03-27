---
title: DLP-Regel für US/UK-Passport-Nummer nicht funktionsfähig
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977105"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Probleme mit DLP-US/UK-Passport-Nummern

**Wichtig**: in diesen noch nie dagewesenen Zeiten werden Maßnahmen ergriffen, um sicherzustellen, dass SharePoint Online-und OneDrive-Dienste hoch verfügbar bleiben – weitere Informationen finden Sie unter [SharePoint Online Anpassungen temporärer Funktionen](https://aka.ms/ODSPAdjustments) .

**DLP-Probleme mit US/UK-Passport-Nummern**

Haben Sie Probleme mit der **Verhinderung von Datenverlust (DLP)** , die bei der Verwendung eines DLP-Typs für vertrauliche Informationen in O365 nicht für Inhalte mit einer **US/UK-Passport-Nummer** funktioniert? Wenn dies der Fall ist, stellen Sie sicher, dass Ihre Inhalte die erforderlichen Informationen dafür enthalten, wonach die DLP-Richtlinie bei der Auswertung sucht.
  
Für eine **US/UK-Passport-Nummern** Richtlinie, die mit einer Konfidenz Stufe von 75% konfiguriert wurde, werden beispielsweise die folgenden Werte ausgewertet und müssen erkannt werden, damit die Regel ausgelöst wird.
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Neun Ziffern

- **[Muster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Neun aufeinanderfolgende Ziffern

- **[Prüfsumme:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nein, es gibt keine Prüfsumme

- **[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Eine DLP-Richtlinie ist 75% sicher, dass diese Art von vertraulichen Informationen erkannt wurde, wenn Sie in einer Nähe von 300 Zeichen:

  - Die Funktion Func_usa_uk_passport findet Inhalte, die dem Muster entsprechen.

  - Ein Schlüsselwort aus Keyword_passport wurde gefunden.

    Das folgende Beispiel würde beispielsweise für die **US/UK-Passport-Nummern** Richtlinie ausgelöst: U.S. Passport-Nummer 123456789

Weitere Informationen dazu, was erforderlich ist, damit eine US/UK-Passport-Nummer für Ihre Inhalte erkannt wird, finden Sie im folgenden Abschnitt in diesem Artikel: [welche Arten von vertraulichen Informationen suchen nach US/UK Passport-Nummer](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Unter Verwendung eines anderen integrierten vertraulichen Informationstyps finden Sie im folgenden Artikel Informationen darüber, was für andere Typen erforderlich ist: [was die Typen für vertrauliche Informationen suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  