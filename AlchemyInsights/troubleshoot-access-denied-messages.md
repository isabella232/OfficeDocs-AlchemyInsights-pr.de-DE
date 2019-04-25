---
title: Problembehandlung bei Zugriff verweigerten Nachrichten
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: f1a4803838b6511ef4fe7f03cafa4aa13b3c9734
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420699"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="246ed-102">Problembehandlung bei Zugriff verweigerten Nachrichten</span><span class="sxs-lookup"><span data-stu-id="246ed-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="246ed-103">Wenn jemand eine Meldung "Zugriff verweigert" in einem freigegebenen Ordner erhalten hat, hat der Websitesammlungsadministrator möglicherweise den Sperrmodus für Benutzerberechtigungen mit eingeschränktem Zugriff aktiviert.</span><span class="sxs-lookup"><span data-stu-id="246ed-103">If someone got an "Access Denied" message to a shared folder, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="246ed-104">Deaktivieren Sie diese Option:</span><span class="sxs-lookup"><span data-stu-id="246ed-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="246ed-105">Wechseln Sie zur Website, klicken Sie auf das Symbol Einstellungen, und klicken Sie dann auf **Websiteeinstellungen**.</span><span class="sxs-lookup"><span data-stu-id="246ed-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="246ed-106">Klicken Sie unter **Websitesammlungsverwaltung** auf **Websitesammlungsfeatures**.</span><span class="sxs-lookup"><span data-stu-id="246ed-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="246ed-107">Klicken Sie neben dem **Sperrmodus für Benutzer mit eingeschränktem Zugriff**auf **Deaktivieren**.</span><span class="sxs-lookup"><span data-stu-id="246ed-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="246ed-108">Eine Meldung "Zugriff verweigert" kann auch für freigegebene Ordner auftreten, wenn es sich bei der Website um eine Veröffentlichungswebsite handelt.</span><span class="sxs-lookup"><span data-stu-id="246ed-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="246ed-109">Weitere Informationen finden Sie unter [Zugriff verweigert beim Zugriff auf einen freigegebenen Ordner](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="246ed-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="246ed-110">Wenn eine Person beim Versuch, Zugriffsanforderungen anzuzeigen, die Meldung "Zugriff verweigert" erhalten hat, muss der Benutzer entweder als Websitesammlungsadministrator oder als Mitglied der Gruppe "Besitzer" für die Website hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="246ed-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="246ed-111">Weitere Informationen finden Sie unter [Access denied to Access Requests List](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="246ed-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="246ed-112">Wenn ein Benutzer eine Meldung "Zugriff verweigert" erhalten hat, nachdem er aus Active Directory entfernt und dann wieder hinzugefügt wurde, finden Sie weitere Informationen unter [Zugriff verweigert, wenn ein Benutzerkonto mit Office 365 synchronisiert wird](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="246ed-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

