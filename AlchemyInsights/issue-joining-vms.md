---
title: Problem beim Verbinden von VMs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884586"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="57d47-102">Problem beim Verbinden von VMs</span><span class="sxs-lookup"><span data-stu-id="57d47-102">Issue joining VMs</span></span>

<span data-ttu-id="57d47-103">Führen Sie die folgenden Schritte durch, um Probleme zu beheben, die beim Verbinden von VMs auftreten:</span><span class="sxs-lookup"><span data-stu-id="57d47-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="57d47-104">Versuchen Sie, sich mit dem **UPN**-Format (z. B. "joeuser@contoso.com") anstelle des **SAMAccountName**-Formats ("CONTOSO\joeuser") anzumelden.</span><span class="sxs-lookup"><span data-stu-id="57d47-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="57d47-105">Stellen Sie sicher, dass Sie die Kennwortsynchronisierung gemäß den Schritten in der Anleitung *Erste Schritte* aktiviert haben.</span><span class="sxs-lookup"><span data-stu-id="57d47-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="57d47-106">Stellen Sie sicher, dass das betroffene Benutzerkonto kein externes Konto im Azure AD-Mandanten ist.</span><span class="sxs-lookup"><span data-stu-id="57d47-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="57d47-107">Externe Benutzer können sich nicht an der verwalteten Domäne anmelden, da Azure AD Domain Services keine Anmeldeinformationen für solche Benutzerkonten hat.</span><span class="sxs-lookup"><span data-stu-id="57d47-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="57d47-108">Wenn das betroffene Benutzerkonto ein reines Cloud-Benutzerkonto ist, stellen Sie sicher, dass die Benutzer ihr Kennwort geändert haben, nachdem Sie Azure AD Domain Services aktiviert haben.</span><span class="sxs-lookup"><span data-stu-id="57d47-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="57d47-109">Dieser Schritt bewirkt, dass die für Azure AD Domain Services erforderlichen Anmeldeinformations-Hashes generiert werden.</span><span class="sxs-lookup"><span data-stu-id="57d47-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="57d47-110">Wenn die betroffenen Benutzerkonten aus einem lokalen Verzeichnis synchronisiert werden, überprüfen Sie, ob die empfohlene Version von Azure AD Connect so konfiguriert wurde, dass eine vollständige Synchronisierung durchgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="57d47-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="57d47-111">Wenn die Probleme nach der Bestätigung von Schritt 4 weiterhin bestehen, führen Sie die folgenden Befehle von Ihrem Synchronisierungsgerät aus:</span><span class="sxs-lookup"><span data-stu-id="57d47-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="57d47-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="57d47-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>