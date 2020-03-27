---
title: DLP-Regel für US-Bank Kontonummer nicht funktionsfähig
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: bb7d8ca91af73fa4ebed5992ec848128beb18830
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977161"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP-Probleme mit US-Bank Kontonummern

**Wichtig**: in diesen noch nie dagewesenen Zeiten werden Maßnahmen ergriffen, um sicherzustellen, dass SharePoint Online-und OneDrive-Dienste hoch verfügbar bleiben – weitere Informationen finden Sie unter [SharePoint Online Anpassungen temporärer Funktionen](https://aka.ms/ODSPAdjustments) .

**DLP-Probleme mit US-Bank Kontonummern**

Haben Sie Probleme mit der **Verhinderung von Datenverlust (DLP)** , die bei Verwendung eines DLP-Typs für vertrauliche Informationen in O365 nicht für Inhalte mit einer **US-Bank Kontonummer** funktioniert? Wenn dies der Fall ist, stellen Sie sicher, dass Ihre Inhalte die erforderlichen Informationen dafür enthalten, wonach die DLP-Richtlinie bei der Auswertung sucht.
  
Für eine **US-Bank Kontonummern** Richtlinie, die mit einer Konfidenz Stufe von 85% konfiguriert wurde, werden beispielsweise die folgenden Werte ausgewertet und müssen erkannt werden, damit die Regel ausgelöst wird:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 Ziffern

- **[Muster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 aufeinanderfolgende Ziffern.

- **[Prüfsumme:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nein, es gibt keine Prüfsumme

- **[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Eine DLP-Richtlinie ist 75% sicher, dass diese Art von vertraulichen Informationen erkannt wurde, wenn Sie in einer Nähe von 300 Zeichen:

  - Der reguläre Ausdruck Regex_usa_bank_account_number findet Inhalte, die mit dem Muster übereinstimmen.

  - Ein Schlüsselwort aus Keyword_usa_Bank_Account wurde gefunden.

    Das folgende Beispiel würde beispielsweise für die US- **Bank Kontonummern** Richtlinie ausgelöst: Girokonto 78344011

Weitere Informationen darüber, was erforderlich ist, damit eine **US-Bank Kontonummer** für Ihre Inhalte erkannt wird, finden Sie im folgenden Abschnitt in diesem Artikel: [was die Typen für vertrauliche Informationen für die US-Bankkontonummer suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Unter Verwendung eines anderen integrierten vertraulichen Informationstyps finden Sie im folgenden Artikel Informationen darüber, was für andere Typen erforderlich ist: [was die Typen für vertrauliche Informationen suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  