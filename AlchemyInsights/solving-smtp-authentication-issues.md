---
title: Aktivieren von SMTP-Authentifizierung und Problembehandlung
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
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077650"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="f9199-102">Aktivieren von SMTP-Authentifizierung und Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="f9199-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="f9199-103">Wenn Sie die SMTP-Authentifizierung für ein Postfach aktivieren möchten oder beim Versuch, E-Mails durch Authentifizierung eines Geräts oder einer Anwendung bei Microsoft 365 weiterzuleiten, eine Fehlermeldung wie „Client nicht authentifiziert“, „Authentifizierung nicht erfolgreich“ oder „SmtpClientAuthentication“ mit Code 5.7.57, 5.7.3 oder 5.7.139 erhalten, führen Sie die folgenden drei Aktionen durch, um das Problem zu beheben:</span><span class="sxs-lookup"><span data-stu-id="f9199-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="f9199-104">Deaktivieren Sie die [Azure-Sicherheitsstandards](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), indem Sie die Option **Sicherheitsstandards aktivieren** auf **Nein** festlegen.</span><span class="sxs-lookup"><span data-stu-id="f9199-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="f9199-105">a.</span><span class="sxs-lookup"><span data-stu-id="f9199-105">a.</span></span> <span data-ttu-id="f9199-106">Melden Sie sich beim Azure-Portal als Sicherheitsadministrator, Administrator für bedingten Zugriff oder globaler Administrator an.</span><span class="sxs-lookup"><span data-stu-id="f9199-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="f9199-107">b.</span><span class="sxs-lookup"><span data-stu-id="f9199-107">b.</span></span> <span data-ttu-id="f9199-108">Blättern Sie zu „Azure Active Directory“ > **Eigenschaften**.</span><span class="sxs-lookup"><span data-stu-id="f9199-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="f9199-109">c.</span><span class="sxs-lookup"><span data-stu-id="f9199-109">c.</span></span> <span data-ttu-id="f9199-110">Wählen Sie **Sicherheitsstandards verwalten** aus.</span><span class="sxs-lookup"><span data-stu-id="f9199-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="f9199-111">d.</span><span class="sxs-lookup"><span data-stu-id="f9199-111">d.</span></span> <span data-ttu-id="f9199-112">Legen Sie **Sicherheitsstandards aktivieren** auf **Nein** fest.</span><span class="sxs-lookup"><span data-stu-id="f9199-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="f9199-113">e.</span><span class="sxs-lookup"><span data-stu-id="f9199-113">e.</span></span> <span data-ttu-id="f9199-114">Wählen Sie **Speichern** aus.</span><span class="sxs-lookup"><span data-stu-id="f9199-114">Select **Save**.</span></span>

2. <span data-ttu-id="f9199-115">[Aktivieren Sie die SMTP-Clientübermittlung](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) für das lizenzierte Postfach.</span><span class="sxs-lookup"><span data-stu-id="f9199-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="f9199-116">a.</span><span class="sxs-lookup"><span data-stu-id="f9199-116">a.</span></span> <span data-ttu-id="f9199-117">Navigieren Sie im Microsoft 365 Admin Center zu **Aktive Benutzer**, und wählen Sie den Benutzer aus.</span><span class="sxs-lookup"><span data-stu-id="f9199-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="f9199-118">b.</span><span class="sxs-lookup"><span data-stu-id="f9199-118">b.</span></span> <span data-ttu-id="f9199-119">Navigieren Sie zur Registerkarte „E-Mail“, und wählen Sie unter **E-Mail-Apps** die Option **E-Mail-Apps verwalten** aus.</span><span class="sxs-lookup"><span data-stu-id="f9199-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="f9199-120">d.</span><span class="sxs-lookup"><span data-stu-id="f9199-120">d.</span></span> <span data-ttu-id="f9199-121">Stellen Sie sicher, dass **Authentifiziertes SMTP** ausgewählt (aktiviert) ist.</span><span class="sxs-lookup"><span data-stu-id="f9199-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="f9199-122">e.</span><span class="sxs-lookup"><span data-stu-id="f9199-122">e.</span></span> <span data-ttu-id="f9199-123">Wählen Sie **Änderungen speichern** aus.</span><span class="sxs-lookup"><span data-stu-id="f9199-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="f9199-124">[Deaktivieren Sie die mehrstufige Authentifizierung (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) für das lizenzierte Postfach.</span><span class="sxs-lookup"><span data-stu-id="f9199-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="f9199-125">a.</span><span class="sxs-lookup"><span data-stu-id="f9199-125">a.</span></span> <span data-ttu-id="f9199-126">Wechseln Sie zum Microsoft 365 Admin Center, und wählen Sie im linken Navigationsmenü **Benutzer** > **Aktive Benutzer** aus.</span><span class="sxs-lookup"><span data-stu-id="f9199-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="f9199-127">b.</span><span class="sxs-lookup"><span data-stu-id="f9199-127">b.</span></span> <span data-ttu-id="f9199-128">Wählen Sie **Mehrstufige Authentifizierung** aus.</span><span class="sxs-lookup"><span data-stu-id="f9199-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="f9199-129">c.</span><span class="sxs-lookup"><span data-stu-id="f9199-129">c.</span></span> <span data-ttu-id="f9199-130">Wählen Sie den Benutzer aus, und deaktivieren Sie **Mehrstufige Authentifizierung**.</span><span class="sxs-lookup"><span data-stu-id="f9199-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
