---
title: Verwenden einer Wix-Website mit von Office 365 gekauften oder verwalteten Domänen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: ef2e7278b1a70aedca1b2ad9c13c249bf8b09c00
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825946"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Verwenden einer Wix-Website mit von Office 365 gekauften oder verwalteten Domänen

- [Aktualisieren von DNS-Einträgen, um die Website beim aktuellen Hostinganbieter zu belassen](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Der Wix-Artikel "Deine Domain per Weiterleitung mit Wix verbinden" empfiehlt die Verwendung von Verweisen (Hinzufügen von DNS-Einträgen über den obigen Link), anstatt Nameserver zu ändern, wenn Sie Office 365 verwenden.
- Wenn Sie sich dennoch dafür entscheiden, Namenserver auf Wix umzustellen, müssen Sie  [DNS-Einträge bei Wix für Microsoft erstellen](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Bei von Microsoft gekauften Domänen können die Namenserver nicht geändert werden. Wenn Sie die Namenserver ändern müssen, muss die von Microsoft erworbene Domäne  [nach 60 Tagen an einen anderen Hostinganbieter übertragen werden](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)