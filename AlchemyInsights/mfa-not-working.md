---
title: Probleme mit MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810483"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="4fb34-102">Probleme mit Azure MFA</span><span class="sxs-lookup"><span data-stu-id="4fb34-102">Issues with Azure MFA</span></span>
<span data-ttu-id="4fb34-103">Es gibt einige Dinge, die überprüft werden müssen, ob sich Benutzer nicht mit der mehrstufigen Authentifizierung (MFA) anmelden können.</span><span class="sxs-lookup"><span data-stu-id="4fb34-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="4fb34-104">Der betroffene Benutzer wird möglicherweise im Azure Active Directory-Portal blockiert.</span><span class="sxs-lookup"><span data-stu-id="4fb34-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="4fb34-105">In diesem Fall werden Authentifizierungsversuche für den jeweiligen Benutzer automatisch verweigert.</span><span class="sxs-lookup"><span data-stu-id="4fb34-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="4fb34-106">Führen Sie die Schritte in diesem Artikel aus, um die Blockierung zu aufheben.</span><span class="sxs-lookup"><span data-stu-id="4fb34-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="4fb34-107">Wenn die Sperrung des Benutzers nicht hilfreich war oder der Benutzer nicht blockiert ist, können Sie versuchen, MFA für den Benutzer zurückzusetzen, und er wird den Registrierungsprozess erneut durchgehen.</span><span class="sxs-lookup"><span data-stu-id="4fb34-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="4fb34-108">Führen Sie die Schritte in diesem Artikel aus.</span><span class="sxs-lookup"><span data-stu-id="4fb34-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="4fb34-109">Wenn Dies das erste Mal ist, dass Sie MFA aktiviert haben und Sich Ihre Benutzer nicht bei Nicht-Browser-Clients wie Outlook, Skype usw. anmelden können, ist möglicherweise ADAL (Active Directory Authentication Library) für Ihr O365-Abonnement nicht aktiviert.</span><span class="sxs-lookup"><span data-stu-id="4fb34-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="4fb34-110">In diesem Fall müssen Sie eine Verbindung mit Exchange Online Powershell herstellen und dieses Cmdlet ausführen:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="4fb34-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>