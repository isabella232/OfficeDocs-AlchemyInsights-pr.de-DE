---
title: Mehrere Objekte haben die gleiche E-Mail-Adresse als Identität
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431404"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="9b1e7-102">Mehrere Objekte haben die gleiche E-Mail-Adresse als Identität</span><span class="sxs-lookup"><span data-stu-id="9b1e7-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="9b1e7-103">**Mehrere Objekte**</span><span class="sxs-lookup"><span data-stu-id="9b1e7-103">**Multiple objects**</span></span>

<span data-ttu-id="9b1e7-104">Einer häufiger Grund für diesen Fehler ist, dass eine Outlook Web Access-Anforderung bei Vorhandensein mehrerer Objekte mit derselben E-Mail-Adresse als Identität nicht korrekt weitergeleitet werden kann.</span><span class="sxs-lookup"><span data-stu-id="9b1e7-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="9b1e7-105">Um diese Objekte zu finden, führen Sie die folgenden Befehle aus:</span><span class="sxs-lookup"><span data-stu-id="9b1e7-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="9b1e7-106">· Get-Recipient <email address></span><span class="sxs-lookup"><span data-stu-id="9b1e7-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="9b1e7-107">· Get-User <email address></span><span class="sxs-lookup"><span data-stu-id="9b1e7-107">· Get-User <email address></span></span>

<span data-ttu-id="9b1e7-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="9b1e7-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="9b1e7-109">· Get-Contact <email address></span><span class="sxs-lookup"><span data-stu-id="9b1e7-109">· Get-Contact <email address></span></span>

<span data-ttu-id="9b1e7-110">· Get-Mailbox <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="9b1e7-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="9b1e7-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="9b1e7-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="9b1e7-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="9b1e7-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="9b1e7-113">Um das Problem zu beheben, entfernen Sie mehrere Objekte mit derselben E-Mail-Identität, und stellen Sie sicher, dass es immer nur ein einziges Objekt mit einer bestimmten E-Mail-Identität gibt und dass sein Empfängertyp "UserMailbox" ist.</span><span class="sxs-lookup"><span data-stu-id="9b1e7-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="9b1e7-114">**Dieselbe Adresse wird für Postfächer von Unternehmen und Privatpersonen verwendet**</span><span class="sxs-lookup"><span data-stu-id="9b1e7-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="9b1e7-115">Eine weitere Ursache ist, wenn dieselbe Adresse für Postfächer von Unternehmen und Privatkunden verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="9b1e7-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="9b1e7-116">In diesem Fall muss der Benutzer seinen primären Verbraucheralias ändern, bis Cafe dieses Szenario unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9b1e7-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="9b1e7-117">Dies ist ein permanenter Fehler, der nicht ohne Intervention verschwindet.</span><span class="sxs-lookup"><span data-stu-id="9b1e7-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="9b1e7-118">Ausführliche Informationen finden Sie unter [Ändern der E-Mail-Adresse oder Telefonnummer für Ihr Microsoft-Konto](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="9b1e7-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>