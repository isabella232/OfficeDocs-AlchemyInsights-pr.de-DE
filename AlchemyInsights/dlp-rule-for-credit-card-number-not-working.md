---
title: DLP-Regel für Kreditkartennummer nicht funktionsfähig
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932442"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP-Probleme mit Kreditkartennummern

**Wichtig**: viele SharePoint Online-und OneDrive-Kunden führen geschäftskritische Anwendungen für den Dienst aus, der im Hintergrund ausgeführt wird. Dazu gehören Inhaltsmigration, Verhinderung von Datenverlusten (Data Loss Prevention, DLP) und Sicherungslösungen. In diesen noch nie dagewesenen Zeiten machen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online- und OneDrive-Dienste für Ihre Benutzer, die von dem Dienst in Remotearbeitsszenarien mehr denn je abhängig sind, weiterhin hochgradig verfügbar und zuverlässig sind.

Zur Unterstützung dieses Ziels haben wir strengere Drosselungsgrenzen für Hintergrundanwendungen (Migration, DLP und Sicherungslösungen) während der Tageszeit unter der Woche eingeführt. Sie sollten davon ausgehen, dass diese Apps in diesen Zeiten einen sehr begrenzten Durchsatz erreichen. Während der Abendstunden und an Wochenenden wird der Dienst für die Region jedoch in der Lage sein, ein erheblich höheres Volumen an Anforderungen von Hintergrundanwendungen zu verarbeiten.

**DLP-Probleme mit Kreditkartennummern**

Haben Sie Probleme mit der **Verhinderung von Datenverlust (DLP)** , die bei Verwendung eines DLP-Typs für vertrauliche Informationen in O365 nicht für Inhalte mit einer **Kreditkartennummer** funktioniert? Wenn dies der Fall ist, stellen Sie sicher, dass Ihre Inhalte die erforderlichen Informationen enthalten, um die DLP-Richtlinie auszulösen, wenn Sie ausgewertet wird. Für eine **Kreditkarten Richtlinie** , die mit einer Konfidenz Stufe von 85% konfiguriert ist, werden beispielsweise die folgenden Werte ausgewertet und müssen erkannt werden, damit die Regel ausgelöst wird:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 Ziffern, die formatiert oder unformatiert (dddddddddddddddd) sein können und den Luhn-Test bestehen müssen.

- **[Muster:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Sehr komplexes und robustes Muster, das Karten von allen wichtigen Marken weltweit erkennt, einschließlich Visa, Mastercard, Discover Card, JCB, American Express, Geschenkkarten und Diner Cards.

- **[Prüfsumme:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Ja, die Luhn-Prüfsumme

- **[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Eine DLP-Richtlinie ist 85% sicher, dass diese Art von vertraulichen Informationen erkannt wurde, wenn Sie in einer Nähe von 300 Zeichen:

  - Die Funktion Func_credit_card findet Inhalte, die dem Muster entsprechen.

  - Eine der folgenden Bedingungen trifft zu:

  - Ein Schlüsselwort aus Keyword_cc_verification wurde gefunden.

  - Ein Schlüsselwort aus Keyword_cc_name wurde gefunden.

  - Die Funktion Func_expiration_date findet ein Datum im richtigen Datumsformat.

  - Die Prüfsummen Übergabe

    Beispielsweise würde das folgende Beispiel für eine DLP-Kreditkartennummern Richtlinie ausgelöst werden:

  - Visa: 4485 3647 3952 7352
  
  - Gültig bis: 2/2009

Weitere Informationen dazu, was erforderlich ist, damit eine **Kreditkartennummer** für Ihre Inhalte erkannt wird, finden Sie im folgenden Abschnitt in diesem Artikel: [was die Typen für vertrauliche Informationen für Kreditkarte suchen #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Unter Verwendung eines anderen integrierten vertraulichen Informationstyps finden Sie im folgenden Artikel Informationen darüber, was für andere Typen erforderlich ist: [was die Typen für vertrauliche Informationen suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  