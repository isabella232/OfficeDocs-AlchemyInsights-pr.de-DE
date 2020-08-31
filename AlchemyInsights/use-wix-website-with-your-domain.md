---
title: Verwenden einer Wix-Website mit von Office 365 gekauften oder verwalteten Domänen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: 522392d41aa8f84f1f4684ccdbd37d68636be07e
ms.sourcegitcommit: cbed17334557c1dfa471623f8d5e735f72e697da
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/28/2020
ms.locfileid: "47300704"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a><span data-ttu-id="7cd5e-102">Verwenden einer Wix-Website mit von Office 365 gekauften oder verwalteten Domänen</span><span class="sxs-lookup"><span data-stu-id="7cd5e-102">Using Wix website with Office 365 purchased or managed domains</span></span>

- [<span data-ttu-id="7cd5e-103">Aktualisieren von DNS-Einträgen, um die Website beim aktuellen Hostinganbieter zu belassen</span><span class="sxs-lookup"><span data-stu-id="7cd5e-103">Update DNS records to keep your website with your current hosting provider</span></span>](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- <span data-ttu-id="7cd5e-104">Der Wix-Artikel "Deine Domain per Weiterleitung mit Wix verbinden" empfiehlt die Verwendung von Verweisen (Hinzufügen von DNS-Einträgen über den obigen Link), anstatt Nameserver zu ändern, wenn Sie Office 365 verwenden.</span><span class="sxs-lookup"><span data-stu-id="7cd5e-104">Wix article "Connecting a Domain to Wix Using the Pointing Method" recommends using pointing (adding DNS records per the above link) rather than changing names servers when using Office 365</span></span>
- <span data-ttu-id="7cd5e-105">Wenn Sie sich dennoch dafür entscheiden, Namenserver auf Wix umzustellen, müssen Sie  [DNS-Einträge bei Wix für Microsoft erstellen](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="7cd5e-105">If you still choose to change name servers to Wix you will then need to  [Create DNS records at Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)</span></span>
- <span data-ttu-id="7cd5e-106">Bei von Microsoft gekauften Domänen können die Namenserver nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="7cd5e-106">If your domain was purchased from Microsoft the name servers cannot be changed.</span></span> <span data-ttu-id="7cd5e-107">Wenn Sie die Namenserver ändern müssen, muss die von Microsoft erworbene Domäne  [nach 60 Tagen an einen anderen Hostinganbieter übertragen werden](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)</span><span class="sxs-lookup"><span data-stu-id="7cd5e-107">If you have to change names servers the Microsoft purchased domain would need to be  [transferred to another hosting provider after 60 days](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)</span></span>