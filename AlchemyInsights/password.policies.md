---
title: Kennwortrichtlinien
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718186"
---
# <a name="password-policies"></a><span data-ttu-id="80361-102">Kennwortrichtlinien</span><span class="sxs-lookup"><span data-stu-id="80361-102">Password policies</span></span>

<span data-ttu-id="80361-103">**Ich habe Probleme mit der Kennwortrichtlinie für einen Benutzer**</span><span class="sxs-lookup"><span data-stu-id="80361-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="80361-104">Die Kennwortrichtlinie für einen Benutzer hängt davon ab, ob der Benutzer nur cloud- oder lokal ist.</span><span class="sxs-lookup"><span data-stu-id="80361-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="80361-105">Nur Cloudbenutzer müssen ein Kennwort auswählen, das den Anforderungen in diesem Artikel entspricht: Kennwortrichtlinien, die nur für [Cloudbenutzerkonten gelten](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="80361-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="80361-106">Lokale Benutzer müssen ein Kennwort auswählen, das den lokalen Anforderungen entspricht.</span><span class="sxs-lookup"><span data-stu-id="80361-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="80361-107">Wenn ein lokaler Benutzer sein Kennwort nicht festlegen kann, überprüfen Sie Ihre lokalen Anforderungen.</span><span class="sxs-lookup"><span data-stu-id="80361-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="80361-108">**Ich weiß nicht, wie Kennwortablaufrichtlinien festgelegt oder überprüft werden.**</span><span class="sxs-lookup"><span data-stu-id="80361-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="80361-109">Sie können die Ablaufrichtlinie für Cloudbenutzer in Ihrem Mandanten mithilfe von PowerShell festlegen und überprüfen.</span><span class="sxs-lookup"><span data-stu-id="80361-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="80361-110">Befolgen Sie die Anweisungen in diesem Artikel: Festlegen oder Überprüfen der Kennwortrichtlinien [mithilfe von PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="80361-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="80361-111">Die Kennwortablaufrichtlinie für lokale Benutzer wird in Ihrem lokalen AD festgelegt.</span><span class="sxs-lookup"><span data-stu-id="80361-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="80361-112">**Weitere hilfreiche Links:**</span><span class="sxs-lookup"><span data-stu-id="80361-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="80361-113">Erste Schritte mit der Kennwortzurücksetzung</span><span class="sxs-lookup"><span data-stu-id="80361-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="80361-114">Problembehandlung durch den Administrator initiierte Kennwortzurücksetzung</span><span class="sxs-lookup"><span data-stu-id="80361-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
