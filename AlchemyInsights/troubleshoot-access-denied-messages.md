---
title: Problembehandlung bei Zugriff verweigerten Nachrichten
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 1930edcfd14acc48ea77b66e2793654a3e6332cc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759799"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="2526e-102">Problembehandlung bei Zugriff verweigerten Nachrichten</span><span class="sxs-lookup"><span data-stu-id="2526e-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="2526e-103">Wenn jemand eine Meldung "Zugriff verweigert" in einem freigegebenen Ordner in SharePoint erhalten hat, hat der Websitesammlungsadministrator möglicherweise den Sperrmodus "eingeschränkter Zugriff auf Benutzerberechtigungen" aktiviert.</span><span class="sxs-lookup"><span data-stu-id="2526e-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="2526e-104">Um dies zu deaktivieren:</span><span class="sxs-lookup"><span data-stu-id="2526e-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="2526e-105">Wechseln Sie zu der Website, klicken Sie auf das Symbol Einstellungen, und klicken Sie dann auf **Websiteeinstellungen**.</span><span class="sxs-lookup"><span data-stu-id="2526e-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="2526e-106">Klicken Sie unter **Websitesammlungsverwaltung** auf **Websitesammlungsfeatures**.</span><span class="sxs-lookup"><span data-stu-id="2526e-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="2526e-107">Klicken Sie neben **Benutzer Berechtigungs Sperrmodus für beschränkte Zugriffs**Rechte auf **Deaktivieren**.</span><span class="sxs-lookup"><span data-stu-id="2526e-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="2526e-108">Eine Nachricht mit Zugriff verweigert kann auch für freigegebene Ordner auftreten, wenn es sich bei der Website um eine Veröffentlichungswebsite handelt.</span><span class="sxs-lookup"><span data-stu-id="2526e-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="2526e-109">Informationen finden Sie unter [Zugriff verweigert beim Zugriff auf einen freigegebenen Ordner](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="2526e-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="2526e-110">Wenn ein Benutzer bei dem Versuch, Zugriffsanforderungen anzuzeigen, eine Meldung "Zugriff verweigert" erhalten hat, muss er als Websitesammlungsadministrator oder als Mitglied der Gruppe "Besitzer" für die Website hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="2526e-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="2526e-111">Weitere Informationen finden Sie unter [Access denied to Access Requests List](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="2526e-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="2526e-112">Wenn ein Benutzer eine Meldung "Zugriff verweigert" erhalten hat, nachdem er aus Active Directory lokal entfernt und anschließend wieder hinzugefügt wurde, finden Sie Informationen unter [Zugriff verweigert, wenn ein Benutzerkonto mit Microsoft 365 synchronisiert wird](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="2526e-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

