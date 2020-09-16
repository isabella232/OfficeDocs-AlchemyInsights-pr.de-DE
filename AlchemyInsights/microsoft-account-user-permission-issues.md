---
title: Problembehandlung – Benutzer wurde nicht im Verzeichnis gefunden
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725406"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="ae465-102">Problembehandlung – Benutzer wurde nicht im Verzeichnis gefunden</span><span class="sxs-lookup"><span data-stu-id="ae465-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="ae465-103">Wenn Benutzer Fehlermeldung "Benutzer kann nicht gefunden werden" im Verzeichnis erhalten, versuchen Sie es erneut, wobei der Problemtyp Benutzer nicht im Verzeichnis ist.</span><span class="sxs-lookup"><span data-stu-id="ae465-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="ae465-104">Die folgenden Schritte können zur Behandlung des Problems ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="ae465-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="ae465-105">Stellen Sie sicher, dass das Konto, mit dem die e-Mail-Einladung angenommen wurde, das gleiche Konto ist, mit dem Sie sich später anmelden.</span><span class="sxs-lookup"><span data-stu-id="ae465-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="ae465-106">Stellen Sie sicher, dass der Benutzer dasselbe Konto verwendet, um die Einladung zu akzeptieren und sich bei der Website anzumelden.</span><span class="sxs-lookup"><span data-stu-id="ae465-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="ae465-107">Weitere Informationen finden Sie unter [Vorgehensweise Verwalten von Aliasen für Ihr Microsoft-Konto </a> zum Verwalten der Microsoft 365-Anmeldung](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="ae465-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="ae465-108">Wechseln Sie zu jedem Standort (en), in dem der Benutzer den Fehler empfängt.</span><span class="sxs-lookup"><span data-stu-id="ae465-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="ae465-109">Fügen Sie "/_layouts/15/people.aspx/membershipgroupid = 0" (innerhalb der Anführungszeichen) an das Ende der Website-URL an.</span><span class="sxs-lookup"><span data-stu-id="ae465-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="ae465-110">Beispiel: https://< "Contoso" >. SharePoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="ae465-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="ae465-111">Wählen Sie den Benutzer aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="ae465-111">Select the user from the list.</span></span>

- <span data-ttu-id="ae465-112">Klicken Sie im Menüband auf **Benutzerberechtigungen entfernen** .</span><span class="sxs-lookup"><span data-stu-id="ae465-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="ae465-113">Fügen Sie den Benutzer wieder hinzu, und senden Sie die Einladung erneut an den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="ae465-113">Add back the User and Resend the invite to the user.</span></span>

