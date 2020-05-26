---
title: Sie möchten eine Domäne oder einen E-Mail-Absender als sicher kennzeichnen?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281147"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Sie möchten eine Domäne oder einen E-Mail-Absender als sicher kennzeichnen?

- Die Verwendung von **Listen sicherer Absender wird nicht empfohlen**, da diese Methode Ihre Organisation für Spam-, Phishing- und Spoofing-Angriffe anfällig macht.
- Ist dies für Ihr Unternehmen jedoch erforderlich, **empfehlen** wir, **[Regeln zur Nachrichtenübermittlung](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** einzurichten. Unsere Anleitung garantiert die Absenderauthentifizierung (stellt sicher, dass die Absenderdomäne nicht verschleiert wurde). **Hinweis**: Es wird nicht empfohlen, falsche Positivmeldungen mithilfe von Listen sicherer Absender zu verwalten, da Ausnahmen der Spamfilterung Ihre Organisation anfällig für Sicherheitsangriffe machen können. Wenn Ihre Benutzer Nachrichten empfangen, die fälschlicherweise als Spam oder Junk-E-Mail gekennzeichnet sind, möchten wir Sie bitten, diese **[Nachrichten und Dateien an Microsoft zu melden](https://protection.office.com/reportsubmission)**.
- Sichere Absender in Outlook, Liste zulässiger Absender oder zulässiger Domänen in Anti-Spam-Richtlinien **sollten vermieden werden**, da diese Absender alle Schutzmaßnahmen zu Spam, Spoofing und Phishing sowie die Absenderauthentifizierung umgehen (SPF, DKIM, DMARC). Diese Methode eignet sich nur für temporäre Tests.
