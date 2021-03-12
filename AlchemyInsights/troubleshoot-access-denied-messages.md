---
title: Behandeln von Zugriffs verweigerten Nachrichten
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704893"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="553f0-102">Behandeln von Zugriffs verweigerten Nachrichten</span><span class="sxs-lookup"><span data-stu-id="553f0-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="553f0-103">Wenn jemand eine "Zugriff verweigert"-Nachricht an einen freigegebenen Ordner in SharePoint erhalten hat, hat der Websitesammlungsadministrator möglicherweise den Sperrmodus für Benutzerberechtigungen mit eingeschränktem Zugriff aktiviert.</span><span class="sxs-lookup"><span data-stu-id="553f0-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="553f0-104">So deaktivieren Sie dies:</span><span class="sxs-lookup"><span data-stu-id="553f0-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="553f0-105">Navigieren Sie zur Website, klicken Sie auf das Symbol Einstellungen, und klicken Sie dann auf **Websiteeinstellungen**.</span><span class="sxs-lookup"><span data-stu-id="553f0-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="553f0-106">Klicken Sie unter **Websitesammlungsverwaltung** auf **Websitesammlungsfeatures**.</span><span class="sxs-lookup"><span data-stu-id="553f0-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="553f0-107">Klicken Sie neben Sperrmodus für **eingeschränkte Benutzerberechtigungen** auf **Deaktivieren**.</span><span class="sxs-lookup"><span data-stu-id="553f0-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="553f0-108">Eine Nachricht "Zugriff verweigert" kann auch für freigegebene Ordner auftreten, wenn es sich bei der Website um eine Veröffentlichungswebsite handelt.</span><span class="sxs-lookup"><span data-stu-id="553f0-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="553f0-109">Weitere Informationen finden Sie unter [Zugriff verweigert beim Zugriff auf einen freigegebenen Ordner](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span><span class="sxs-lookup"><span data-stu-id="553f0-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="553f0-110">Wenn eine Person beim Anzeigen von Zugriffsanforderungen die Meldung "Zugriff verweigert" erhalten hat, muss der Benutzer entweder als Websitesammlungsadministrator oder als Mitglied der Gruppe Besitzer für die Website hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="553f0-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="553f0-111">Weitere Informationen finden Sie unter [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="553f0-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="553f0-112">Wenn ein Benutzer eine Meldung "Zugriff verweigert" erhalten hat, nachdem er lokal aus Active Directory entfernt und dann wieder hinzugefügt wurde, finden Sie weitere Informationen unter Zugriff verweigert, wenn ein Benutzerkonto mit [Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318)synchronisiert wird.</span><span class="sxs-lookup"><span data-stu-id="553f0-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

