---
title: Teams-Add-in für Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670327"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="4ae1a-102">Teams-Add-in für Mac</span><span class="sxs-lookup"><span data-stu-id="4ae1a-102">Teams add-in for Mac</span></span>

<span data-ttu-id="4ae1a-103">Führen Sie die folgenden Schritte aus, um ein fehlendes Team-Add-in für Benutzende des Mac-Betriebssystems zu beheben:</span><span class="sxs-lookup"><span data-stu-id="4ae1a-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="4ae1a-104">**Schritt 1:** Wenn Sie über Hybrid Exchange On-Premises verfügen (2016 CU3 oder höher erforderlich), verwenden Sie das Tool Test-HMA.ps1, um zu bestätigen, dass die Hybrid Modern Authentication korrekt konfiguriert ist.</span><span class="sxs-lookup"><span data-stu-id="4ae1a-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="4ae1a-105">Weitere Informationen finden Sie unter [Hybrid Modern Authentication für Outlook für iOS und Android validieren](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="4ae1a-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="4ae1a-106">**Hinweis** verwenden Sie das UPN-Adressformat (beispielsweise [username@contoso.com](mailto:username@contoso.com)), nicht domain\username.</span><span class="sxs-lookup"><span data-stu-id="4ae1a-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="4ae1a-107">Tun Sie dies auch für Benutzende mit Exchange Online-Postfächern.</span><span class="sxs-lookup"><span data-stu-id="4ae1a-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="4ae1a-108">**Schritt 2:** Lassen Sie Benutzende in Outlook für Mac auf **Tools** > **Konten** gehen und das Konto suchen und auswählen.</span><span class="sxs-lookup"><span data-stu-id="4ae1a-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="4ae1a-109">Bestätigen Sie, dass der aufgelistete Benutzername im UPN-Format (beispielsweise [username@contoso.com](mailto:username@contoso.com)) ist.</span><span class="sxs-lookup"><span data-stu-id="4ae1a-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="4ae1a-110">**Schritt 3:** Bestätigen Sie, dass die Benutzenden lizenzierte Microsoft Teams-Benutzende sind.</span><span class="sxs-lookup"><span data-stu-id="4ae1a-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="4ae1a-111">Benutzende müssen das Office 365 für Mac-Abonnement, Produktversion 16.24 oder höher, verwenden.</span><span class="sxs-lookup"><span data-stu-id="4ae1a-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>