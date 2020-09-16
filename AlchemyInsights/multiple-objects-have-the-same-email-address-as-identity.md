---
title: Mehrere Objekte haben die gleiche E-Mail-Adresse als Identität
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724614"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="75d0b-102">Mehrere Objekte haben die gleiche E-Mail-Adresse als Identität</span><span class="sxs-lookup"><span data-stu-id="75d0b-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="75d0b-103">**Mehrere Objekte**</span><span class="sxs-lookup"><span data-stu-id="75d0b-103">**Multiple objects**</span></span>

<span data-ttu-id="75d0b-104">Einer häufiger Grund für diesen Fehler ist, dass eine Outlook Web Access-Anforderung bei Vorhandensein mehrerer Objekte mit derselben E-Mail-Adresse als Identität nicht korrekt weitergeleitet werden kann.</span><span class="sxs-lookup"><span data-stu-id="75d0b-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="75d0b-105">Um diese Objekte zu finden, führen Sie die folgenden Befehle aus:</span><span class="sxs-lookup"><span data-stu-id="75d0b-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="75d0b-106">· Get-Recipient <email address></span><span class="sxs-lookup"><span data-stu-id="75d0b-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="75d0b-107">· Get-User <email address></span><span class="sxs-lookup"><span data-stu-id="75d0b-107">· Get-User <email address></span></span>

<span data-ttu-id="75d0b-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="75d0b-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="75d0b-109">· Get-Contact <email address></span><span class="sxs-lookup"><span data-stu-id="75d0b-109">· Get-Contact <email address></span></span>

<span data-ttu-id="75d0b-110">· Get-Mailbox <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="75d0b-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="75d0b-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="75d0b-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="75d0b-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="75d0b-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="75d0b-113">Um das Problem zu beheben, entfernen Sie mehrere Objekte mit derselben E-Mail-Identität, und stellen Sie sicher, dass es immer nur ein einziges Objekt mit einer bestimmten E-Mail-Identität gibt und dass sein Empfängertyp "UserMailbox" ist.</span><span class="sxs-lookup"><span data-stu-id="75d0b-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="75d0b-114">**Dieselbe Adresse wird für Postfächer von Unternehmen und Privatpersonen verwendet**</span><span class="sxs-lookup"><span data-stu-id="75d0b-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="75d0b-115">Eine weitere Ursache ist, wenn dieselbe Adresse für Postfächer von Unternehmen und Privatkunden verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="75d0b-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="75d0b-116">In diesem Fall muss der Benutzer seinen primären Verbraucheralias ändern, bis Cafe dieses Szenario unterstützt.</span><span class="sxs-lookup"><span data-stu-id="75d0b-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="75d0b-117">Dies ist ein permanenter Fehler, der nicht ohne Intervention verschwindet.</span><span class="sxs-lookup"><span data-stu-id="75d0b-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="75d0b-118">Ausführliche Informationen finden Sie unter [Ändern der E-Mail-Adresse oder Telefonnummer für Ihr Microsoft-Konto](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="75d0b-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>