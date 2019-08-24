---
title: Schreibgeschützt für Wartungs Nachrichten beim Versuch, SharePoint oder OneDrive zu verwenden
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620722"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="2e64b-102">Schreibgeschützt für Wartungs Nachrichten beim Versuch, SharePoint oder OneDrive zu verwenden</span><span class="sxs-lookup"><span data-stu-id="2e64b-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="2e64b-103">Benutzer erhalten möglicherweise eine **schreibgeschützte Nachricht für die Wartung** , wenn Sie versuchen, SharePoint oder OneDrive für eines der folgenden Szenarien zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="2e64b-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="2e64b-104">Eine geplante oder aktive Wartungs Aktivität.</span><span class="sxs-lookup"><span data-stu-id="2e64b-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="2e64b-105">Überprüfen Sie diese, indem Sie zum [Nachrichten Center](https://portal.office.com/adminportal/home#/messagecenter)navigieren.</span><span class="sxs-lookup"><span data-stu-id="2e64b-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="2e64b-106">Ein aktiver Dienst Vorfall mit hoher Priorität, der möglicherweise auftritt.</span><span class="sxs-lookup"><span data-stu-id="2e64b-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="2e64b-107">Suchen Sie nach Warnungen/Vorfällen, indem Sie zum [Dienststatus](https://portal.office.com/adminportal/home#/servicehealth)navigieren.</span><span class="sxs-lookup"><span data-stu-id="2e64b-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="2e64b-108">Ein kleines Wiederherstellungsszenario, das aufgrund unerwarteter Ereignisse auf den Servern möglicherweise nicht mehr als 30 Minuten dauern kann.</span><span class="sxs-lookup"><span data-stu-id="2e64b-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="2e64b-109">Es gibt keine Nachrichten Center-oder Dienst Integritäts Beiträge für diese kleinen Wiederherstellungen, aber Sie sollten bald wieder ganz normal sein.</span><span class="sxs-lookup"><span data-stu-id="2e64b-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="2e64b-110">In sehr seltenen Fällen haben wir festgestellt, dass eines der drei oben aufgelisteten Szenarien die Ursache war, und der Dienst wurde wiederhergestellt, aber der Browsercache für Benutzer wurde nicht gelöscht.</span><span class="sxs-lookup"><span data-stu-id="2e64b-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="2e64b-111">Versuchen Sie, den Browsercache zu löschen, bevor Sie zur Website navigieren.</span><span class="sxs-lookup"><span data-stu-id="2e64b-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="2e64b-112">Wählen Sie in Ihrem Microsoft Edge-Browser **Einstellungen**aus, und wählen Sie dann **Datenschutz und Sicherheit**aus.</span><span class="sxs-lookup"><span data-stu-id="2e64b-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="2e64b-113">Wählen Sie unter **Browser löschen** **die Option zu Lösch**Ende Elemente auswählen aus.</span><span class="sxs-lookup"><span data-stu-id="2e64b-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="2e64b-114">Wählen Sie **Cookies und gespeicherte Website Daten**aus, und wählen Sie **Löschen**aus.</span><span class="sxs-lookup"><span data-stu-id="2e64b-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="2e64b-115">Diese Schritte können unterschiedlich sein, wenn Sie andere Browser wie Mozilla Firefox oder Google Chrome verwenden.</span><span class="sxs-lookup"><span data-stu-id="2e64b-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="2e64b-116">Eine weitere Option besteht darin, Ihre SharePoint-Website oder OneDrive in einem neuen InPrivate-Fenster zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="2e64b-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>