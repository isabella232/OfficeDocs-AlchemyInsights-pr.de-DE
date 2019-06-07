---
title: Erstellen und Verwenden eines freigegebenen Postfachs
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81bf8082198de1c44037291f23c434d06a77f02a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762400"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="0c0e7-102">Problembehandlung – Benutzer wurde nicht im Verzeichnis gefunden</span><span class="sxs-lookup"><span data-stu-id="0c0e7-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="0c0e7-103">Wenn Benutzer Fehlermeldung "Benutzer kann nicht gefunden werden" im Verzeichnis empfangen.</span><span class="sxs-lookup"><span data-stu-id="0c0e7-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="0c0e7-104">Versuchen Sie es erneut, wobei der Problemtyp Benutzer nicht im Verzeichnis ist.</span><span class="sxs-lookup"><span data-stu-id="0c0e7-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="0c0e7-105">Die folgenden Schritte können zur Behandlung des Problems ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="0c0e7-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="0c0e7-106">Stellen Sie sicher, dass das Konto, mit dem die e-Mail-Einladung angenommen wurde, das gleiche Konto ist, mit dem Sie sich später anmelden.</span><span class="sxs-lookup"><span data-stu-id="0c0e7-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="0c0e7-107">Stellen Sie sicher, dass der Benutzer dasselbe Konto verwendet, um die Einladung zu akzeptieren und sich bei der Website anzumelden.</span><span class="sxs-lookup"><span data-stu-id="0c0e7-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="0c0e7-108">Weitere Informationen finden Sie unter [Vorgehensweise Verwalten von Aliasen für</a> Ihr Microsoft-Konto zum Verwalten der Office 365 Anmeldung](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="0c0e7-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="0c0e7-109">Wechseln Sie zu jedem Standort (en), in dem der Benutzer den Fehler empfängt.</span><span class="sxs-lookup"><span data-stu-id="0c0e7-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="0c0e7-110">Fügen Sie "/_layouts/15/people.aspx/membershipgroupid = 0" (innerhalb der Anführungszeichen) am Ende der Website-URL hinzu.</span><span class="sxs-lookup"><span data-stu-id="0c0e7-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="0c0e7-111">Beispiel: https://#a0 "Contoso" #a1. SharePoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="0c0e7-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="0c0e7-112">Wählen Sie den Benutzer aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="0c0e7-112">Select the user from the list.</span></span>

- <span data-ttu-id="0c0e7-113">Klicken Sie im Menüband auf **Benutzerberechtigungen entfernen** .</span><span class="sxs-lookup"><span data-stu-id="0c0e7-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="0c0e7-114">Fügen Sie den Benutzer wieder hinzu, und senden Sie die Einladung erneut an den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="0c0e7-114">Add back the User and Resend the invite to the user.</span></span>

