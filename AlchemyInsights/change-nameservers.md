---
title: Ändern von Namenservern
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 07a0dd19a768dd2b97923f0ced566b69ca2d6ba7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47714687"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="4d11f-102">Aktualisieren Ihrer Domänennamenserver, sodass sie auf Microsoft verweisen</span><span class="sxs-lookup"><span data-stu-id="4d11f-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="4d11f-103">Hinweis: Die Verarbeitung von Änderungen an Nameservern kann manchmal bis zu 48 Stunden dauern.</span><span class="sxs-lookup"><span data-stu-id="4d11f-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="4d11f-p101">Zum Einrichten Ihrer Domäne in Microsoft 365 müssen die Namenserver Ihrer Registrierungsstelle aktualisiert werden. Erstellen oder bearbeiten Sie Ihre Namenservereinträge Ihrer Domänenregistrierungsstelle.</span><span class="sxs-lookup"><span data-stu-id="4d11f-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="4d11f-106">Navigieren Sie zur Website Ihrer Domänenregistrierungsstelle, und suchen Sie den Bereich, in dem Sie die Namenserver bearbeiten können.</span><span class="sxs-lookup"><span data-stu-id="4d11f-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="4d11f-107">Erstellen oder bearbeiten Sie zwei Namenservereinträge so, dass sie diesen Werten entsprechen:</span><span class="sxs-lookup"><span data-stu-id="4d11f-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="4d11f-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="4d11f-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="4d11f-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="4d11f-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="4d11f-110">Speichern Sie die Änderungen.</span><span class="sxs-lookup"><span data-stu-id="4d11f-110">Save changes.</span></span>

<span data-ttu-id="4d11f-111">Detaillierte Anweisungen finden Sie auch in diesem Artikel: [Ändern von Namenservern mit einer beliebigen Domänenregistrierungsstelle](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="4d11f-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  