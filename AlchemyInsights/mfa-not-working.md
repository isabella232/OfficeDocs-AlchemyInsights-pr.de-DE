---
title: Probleme mit MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36545164"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="3a44b-102">Probleme mit MFA</span><span class="sxs-lookup"><span data-stu-id="3a44b-102">Issues with MFA</span></span>
<span data-ttu-id="3a44b-103">Es gibt einige Dinge, die überprüft werden müssen, wenn sich Benutzer nicht mit mehrstufiger Authentifizierung (MFA) anmelden können.</span><span class="sxs-lookup"><span data-stu-id="3a44b-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="3a44b-104">Der betroffene Benutzer wird möglicherweise in Azure Active Directory-Portal blockiert.</span><span class="sxs-lookup"><span data-stu-id="3a44b-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="3a44b-105">Wenn dies der Fall ist, werden Authentifizierungsversuche für diesen bestimmten Benutzer automatisch verweigert.</span><span class="sxs-lookup"><span data-stu-id="3a44b-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="3a44b-106">Führen Sie die Schritte in diesem Artikel aus, um die Blockierung aufzuheben.</span><span class="sxs-lookup"><span data-stu-id="3a44b-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="3a44b-107">Wenn die Blockierung des Benutzers aufgehoben wurde oder der Benutzer nicht blockiert ist, können Sie versuchen, MFA für den Benutzer zurückzusetzen, und Sie werden den Registrierungsprozess erneut durchlaufen.</span><span class="sxs-lookup"><span data-stu-id="3a44b-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="3a44b-108">Führen Sie die Schritte in diesem Artikel aus.</span><span class="sxs-lookup"><span data-stu-id="3a44b-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="3a44b-109">Wenn Sie das erste Mal MFA aktiviert haben und sich Ihre Benutzer nicht für Clients wie Outlook, Skype usw. anmelden können, die möglicherweise Adal (Active Directory Authentifizierungsbibliothek) in Ihrem O365-Abonnement nicht aktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="3a44b-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="3a44b-110">In diesem Fall müssen Sie eine Verbindung mit Exchange Online PowerShell herstellen und dieses Cmdlet ausführen:  *festlegen-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="3a44b-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>