---
title: Eines Ihrer lokalen Verbunddienst Zertifikate läuft ab
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 24c369c61ad7cf7a9fe101ac29271c32e5159c1f
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761382"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="c4709-102">Eines Ihrer lokalen Verbunddienst Zertifikate läuft ab</span><span class="sxs-lookup"><span data-stu-id="c4709-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="c4709-103">Führen Sie die folgenden Schritte aus, um dieses Problem zu beheben:</span><span class="sxs-lookup"><span data-stu-id="c4709-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="c4709-104">Installieren Sie das Microsoft Azure Active Directory Modul für Windows PowerShell auf dem Computer (falls das Modul noch nicht installiert ist).</span><span class="sxs-lookup"><span data-stu-id="c4709-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="c4709-105">Wechseln Sie dazu zu [Azure Active Directory PowerShell for Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="c4709-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="c4709-106">Befolgen Sie die Schritte im Abschnitt "Szenario 1: abgelaufenes AD FS-Token-Signierungszertifikat" unter ["Fehler beim Zugriff auf die Website" von AD FS, wenn sich ein Verbundbenutzer bei Office 365, Azure oder InTune anmeldet](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="c4709-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="c4709-107">Befolgen Sie die Schritte in t[So aktualisieren oder reparieren Sie die Einstellungen einer Verbunddomäne in Office 365, Azure oder InTune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="c4709-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="c4709-108">Weitere Informationen zum Erneuern von Verbund Zertifikaten finden Sie unter [Zertifikaterneuerung für O365 und Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="c4709-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

