---
title: Ändern von Namenservern
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 67680a6fa514d31ccb88cc8691a199cd1f58a402
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818611"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="825d3-102">Aktualisieren Ihrer Domänennamenserver, sodass sie auf Microsoft verweisen</span><span class="sxs-lookup"><span data-stu-id="825d3-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="825d3-103">Hinweis: Die Verarbeitung von Änderungen an Nameservern kann manchmal bis zu 48 Stunden dauern.</span><span class="sxs-lookup"><span data-stu-id="825d3-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="825d3-p101">Zum Einrichten Ihrer Domäne in Microsoft 365 müssen die Namenserver Ihrer Registrierungsstelle aktualisiert werden. Erstellen oder bearbeiten Sie Ihre Namenservereinträge Ihrer Domänenregistrierungsstelle.</span><span class="sxs-lookup"><span data-stu-id="825d3-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="825d3-106">Navigieren Sie zur Website Ihrer Domänenregistrierungsstelle, und suchen Sie den Bereich, in dem Sie die Namenserver bearbeiten können.</span><span class="sxs-lookup"><span data-stu-id="825d3-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="825d3-107">Erstellen oder bearbeiten Sie zwei Namenservereinträge so, dass sie diesen Werten entsprechen:</span><span class="sxs-lookup"><span data-stu-id="825d3-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="825d3-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="825d3-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="825d3-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="825d3-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="825d3-110">Speichern Sie die Änderungen.</span><span class="sxs-lookup"><span data-stu-id="825d3-110">Save changes.</span></span>

<span data-ttu-id="825d3-111">Detaillierte Anweisungen finden Sie auch in diesem Artikel: [Ändern von Namenservern mit einer beliebigen Domänenregistrierungsstelle](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="825d3-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  