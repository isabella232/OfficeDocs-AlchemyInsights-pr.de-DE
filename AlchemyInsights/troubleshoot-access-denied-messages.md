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
ms.openlocfilehash: e4fea7188bd77ba876e2a245414372c3ff836059
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500402"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="6a615-102">Problembehandlung bei Zugriff verweigerten Nachrichten</span><span class="sxs-lookup"><span data-stu-id="6a615-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="6a615-103">Wenn jemand eine Meldung "Zugriff verweigert" in einem freigegebenen Ordner in SharePoint erhalten hat, hat der Websitesammlungsadministrator möglicherweise den Sperrmodus "eingeschränkter Zugriff auf Benutzerberechtigungen" aktiviert.</span><span class="sxs-lookup"><span data-stu-id="6a615-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="6a615-104">Um dies zu deaktivieren:</span><span class="sxs-lookup"><span data-stu-id="6a615-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="6a615-105">Wechseln Sie zu der Website, klicken Sie auf das Symbol Einstellungen, und klicken Sie dann auf **Websiteeinstellungen**.</span><span class="sxs-lookup"><span data-stu-id="6a615-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="6a615-106">Klicken Sie unter **Websitesammlungsverwaltung** auf **Websitesammlungsfeatures**.</span><span class="sxs-lookup"><span data-stu-id="6a615-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="6a615-107">Klicken Sie neben **Benutzer Berechtigungs Sperrmodus für beschränkte Zugriffs**Rechte auf **Deaktivieren**.</span><span class="sxs-lookup"><span data-stu-id="6a615-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="6a615-108">Eine Nachricht mit Zugriff verweigert kann auch für freigegebene Ordner auftreten, wenn es sich bei der Website um eine Veröffentlichungswebsite handelt.</span><span class="sxs-lookup"><span data-stu-id="6a615-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="6a615-109">Informationen finden Sie unter [Zugriff verweigert beim Zugriff auf einen freigegebenen Ordner](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="6a615-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="6a615-110">Wenn ein Benutzer bei dem Versuch, Zugriffsanforderungen anzuzeigen, eine Meldung "Zugriff verweigert" erhalten hat, muss er als Websitesammlungsadministrator oder als Mitglied der Gruppe "Besitzer" für die Website hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="6a615-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="6a615-111">Weitere Informationen finden Sie unter [Access denied to Access Requests List](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="6a615-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="6a615-112">Wenn ein Benutzer eine Meldung "Zugriff verweigert" erhalten hat, nachdem er aus Active Directory lokal entfernt und anschließend wieder hinzugefügt wurde, finden Sie Informationen unter [Zugriff verweigert, wenn ein Benutzerkonto mit Office 365 synchronisiert wird](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="6a615-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

