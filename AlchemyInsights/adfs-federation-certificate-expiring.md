---
title: AD FS-Verbund Zertifikat abläuft.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: c608489be8497233d9d4f87ec53649026b823250
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28289449"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="de1a8-102">AD FS-Verbund Zertifikat abläuft.</span><span class="sxs-lookup"><span data-stu-id="de1a8-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="de1a8-103">Gehen Sie folgendermaßen vor, um dieses Problem zu beheben:</span><span class="sxs-lookup"><span data-stu-id="de1a8-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="de1a8-p101">Installieren Sie die Microsoft Azure Active Directory-Modul für Windows PowerShell auf dem Computer (sofern das Modul nicht bereits installiert ist). Wechseln Sie zu diesem Zweck zum [Verwalten von Azure Active Directory mithilfe von Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="de1a8-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>
    
2. <span data-ttu-id="de1a8-106">Führen Sie die Schritte in der "Szenario 1: die AD FS Tokensignaturzertifikat abgelaufen" im Abschnitt ["Ist ein Problem aufgetreten, den Zugriff auf die Website" Fehler von AD FS, wenn ein Verbundbenutzer bei Office 365, Azure, oder Intune anmeldet](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="de1a8-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
3. <span data-ttu-id="de1a8-107">Führen Sie die Schritte [zum Aktualisieren oder reparieren die Einstellungen einer verbunddomäne in Office 365, Azure, oder Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="de1a8-107">Follow the steps in [How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
    <span data-ttu-id="de1a8-108">Weitere Informationen zum Erneuern von Zertifikaten für den Verbund finden Sie unter [Erneuern von Zertifikaten für Office 365 und Azure Active Directory Federation](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="de1a8-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
    

