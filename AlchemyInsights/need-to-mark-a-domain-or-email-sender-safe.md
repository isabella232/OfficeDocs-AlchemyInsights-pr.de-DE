---
title: Sie möchten eine Domäne oder einen E-Mail-Absender als sicher kennzeichnen?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803244"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="74636-102">Sie möchten eine Domäne oder einen E-Mail-Absender als sicher kennzeichnen?</span><span class="sxs-lookup"><span data-stu-id="74636-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="74636-103">Die Verwendung von **Listen sicherer Absender wird nicht empfohlen**, da diese Methode Ihre Organisation für Spam-, Phishing- und Spoofing-Angriffe anfällig macht.</span><span class="sxs-lookup"><span data-stu-id="74636-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="74636-104">Ist dies für Ihr Unternehmen jedoch erforderlich, **empfehlen** wir, **[Regeln zur Nachrichtenübermittlung](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** einzurichten.</span><span class="sxs-lookup"><span data-stu-id="74636-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="74636-105">Unsere Anleitung garantiert die Absenderauthentifizierung (stellt sicher, dass die Absenderdomäne nicht verschleiert wurde).</span><span class="sxs-lookup"><span data-stu-id="74636-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="74636-106">**Hinweis**: Es wird nicht empfohlen, falsche Positivmeldungen mithilfe von Listen sicherer Absender zu verwalten, da Ausnahmen der Spamfilterung Ihre Organisation anfällig für Sicherheitsangriffe machen können.</span><span class="sxs-lookup"><span data-stu-id="74636-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="74636-107">Wenn Ihre Benutzer Nachrichten empfangen, die fälschlicherweise als Spam oder Junk-E-Mail gekennzeichnet sind, möchten wir Sie bitten, diese **[Nachrichten und Dateien an Microsoft zu melden](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="74636-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="74636-108">Sichere Absender in Outlook, Liste zulässiger Absender oder zulässiger Domänen in Anti-Spam-Richtlinien **sollten vermieden werden**, da diese Absender alle Schutzmaßnahmen zu Spam, Spoofing und Phishing sowie die Absenderauthentifizierung umgehen (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="74636-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="74636-109">Diese Methode eignet sich nur für temporäre Tests.</span><span class="sxs-lookup"><span data-stu-id="74636-109">This method is best used for temporary testing only.</span></span>
