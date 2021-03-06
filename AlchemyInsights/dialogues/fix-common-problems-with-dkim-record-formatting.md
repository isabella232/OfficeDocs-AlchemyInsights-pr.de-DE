---
title: Beheben häufiger Probleme bei der Formatierung von DKIM-Eintragen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50501055"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="6802d-102">Beheben häufiger Probleme bei der Formatierung von DKIM-Eintragen</span><span class="sxs-lookup"><span data-stu-id="6802d-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="6802d-103">Die meisten DkIM-Einrichtungsprobleme stehen im Zusammenhang mit falschen DNS-Einträgen.</span><span class="sxs-lookup"><span data-stu-id="6802d-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="6802d-104">Um die #A0 zu beheben, stellen Sie sicher, dass der DKIM-CNAME-Eintrag **(kein** #A1) richtig formatiert ist.</span><span class="sxs-lookup"><span data-stu-id="6802d-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="6802d-105">Weitere Informationen finden Sie unter Was Sie zum manuellen Einrichten von [DKIM in Office 365 tun müssen.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)</span><span class="sxs-lookup"><span data-stu-id="6802d-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="6802d-106">Wenn Sie Hilfe bei DNS-Einträgen im Allgemeinen benötigen, lesen Sie Erstellen von [DNS-Einträgen bei einem beliebigen DNS-Hostinganbieter für Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span><span class="sxs-lookup"><span data-stu-id="6802d-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="6802d-107">Nachdem Sie Ihre DKIM-DNS-Einträge beim DNS-Hostingdienst für Ihre Domäne erstellt oder aktualisiert haben, müssen Sie warten, bis die DNS-Einträge veröffentlicht werden.</span><span class="sxs-lookup"><span data-stu-id="6802d-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
