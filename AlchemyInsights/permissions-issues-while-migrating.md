---
title: Berechtigungsprobleme während der Migration
ms.author: kirks
author: Techwriter40
ms.date: 9/18/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 3cdf5909595b5b1fac9aeb00865546c1dcff5f09
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32372163"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="c05d5-102">Benutzerprofil-und Fotosynchronisierung</span><span class="sxs-lookup"><span data-stu-id="c05d5-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="c05d5-103">**Profilfoto Synchronisierung** – Benutzer können feststellen, dass Ihr Profilfoto nicht mit SharePoint synchronisiert wird.</span><span class="sxs-lookup"><span data-stu-id="c05d5-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="c05d5-104">Sie haben möglicherweise versucht, Ihr Profilfoto zu aktualisieren, und das Foto wird weiterhin als altes Foto angezeigt.</span><span class="sxs-lookup"><span data-stu-id="c05d5-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="c05d5-105">Um sicherzustellen, dass das Profilfoto wie erwartet angezeigt wird, muss der Benutzer eine Fotosynchronisierung initiieren.</span><span class="sxs-lookup"><span data-stu-id="c05d5-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="c05d5-106">Weitere Informationen zum Foto Synchronisierungsprozess finden Sie unter [Informationen zur Profilbild Synchronisierung in Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span><span class="sxs-lookup"><span data-stu-id="c05d5-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="c05d5-107">**Profilsynchronisierung** : die Zeit, die zum Abschließen einer Profilsynchronisierung erforderlich ist, hängt von der Anzahl der Änderungen ab, die der AD-Import Auftrag verarbeiten muss.</span><span class="sxs-lookup"><span data-stu-id="c05d5-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="c05d5-108">Wenn es viele Änderungen gibt, hat der Zeitgeberauftrag viel Arbeit, und es dauert länger, bis die Änderungen in der Benutzerprofilanwendung wiedergegeben werden.</span><span class="sxs-lookup"><span data-stu-id="c05d5-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="c05d5-109">Wenn für den Zeitgeberauftrag ein kleiner Arbeitsumfang vorliegt, werden die Änderungen in der Benutzerprofilanwendung deutlich schneller widergespiegelt.</span><span class="sxs-lookup"><span data-stu-id="c05d5-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="c05d5-110">Weitere Informationen zum Profil Synchronisierungsprozess finden Sie unter [Informationen zur Benutzerprofil Synchronisierung in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span><span class="sxs-lookup"><span data-stu-id="c05d5-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="c05d5-111">**Update Profil in Office Tauchen Sie ein** , Benutzer können ihr Office 365-Profil verwalten.</span><span class="sxs-lookup"><span data-stu-id="c05d5-111">**Update Profile in Office Delve** - Delve users can manage their Office 365 Profile.</span></span> <span data-ttu-id="c05d5-112">Weitere Informationen finden Sie unter [anzeigen und Aktualisieren Ihres Profils in Office](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)-vertiefen.</span><span class="sxs-lookup"><span data-stu-id="c05d5-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

