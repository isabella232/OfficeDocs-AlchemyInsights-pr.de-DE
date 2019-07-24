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
ms.openlocfilehash: cc232fba6f502e2b6f282a8c1a1e29221e36b70d
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840514"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="f2015-102">Schreibgeschützt für Wartungs Nachrichten beim Versuch, SharePoint oder OneDrive zu verwenden</span><span class="sxs-lookup"><span data-stu-id="f2015-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="f2015-103">Benutzer erhalten möglicherweise eine **schreibgeschützte Nachricht für die Wartung** , wenn Sie versuchen, SharePoint oder OneDrive zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="f2015-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive.</span></span>  <span data-ttu-id="f2015-104">Wenn ja, überprüfen Sie, ob eine aktive Wartung auf Ihrem Mandanten auftritt, indem Sie zum [Nachrichtencenter](https://portal.office.com/adminportal/home#/MessageCenter)navigieren.</span><span class="sxs-lookup"><span data-stu-id="f2015-104">If so, check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span> <span data-ttu-id="f2015-105">Stellen Sie außerdem sicher, dass Sie das [Service](https://portal.office.com/adminportal/home#/servicehealth) -Integritäts Dashboard überprüfen, um nach eventuell auftretenden Warnungen/Vorfällen zu suchen.</span><span class="sxs-lookup"><span data-stu-id="f2015-105">Also, make sure to check the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) dashboard to check for any advisories/incidents that may be occurring.</span></span>

<span data-ttu-id="f2015-106">Wenn weder im Nachrichten Center noch im Dienst Integritäts Dashboard etwas zur aktuellen Wartung für Ihren Mandanten festgestellt wurde, kann dies ein Problem mit der Browserzwischenspeicherung sein.</span><span class="sxs-lookup"><span data-stu-id="f2015-106">If neither the Message Center or Service Health dashboard have noted anything about current maintenance for your tenant, this may be a browser caching issue.</span></span>

<span data-ttu-id="f2015-107">Versuchen Sie, den Browsercache zu löschen, bevor Sie zur Website navigieren.</span><span class="sxs-lookup"><span data-stu-id="f2015-107">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="f2015-108">Wählen Sie in Ihrem Microsoft Edge-Browser **Einstellungen**aus, und wählen Sie dann **Datenschutz und Sicherheit**aus.</span><span class="sxs-lookup"><span data-stu-id="f2015-108">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="f2015-109">Wählen Sie unter **Browser löschen** **die Option zu Lösch**Ende Elemente auswählen aus.</span><span class="sxs-lookup"><span data-stu-id="f2015-109">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="f2015-110">Wählen Sie **Cookies und gespeicherte Website Daten**aus, und wählen Sie **Löschen**aus.</span><span class="sxs-lookup"><span data-stu-id="f2015-110">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="f2015-111">Diese Schritte können unterschiedlich sein, wenn Sie andere Browser wie Mozilla Firefox oder Google Chrome verwenden.</span><span class="sxs-lookup"><span data-stu-id="f2015-111">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="f2015-112">Eine weitere Option besteht darin, Ihre SharePoint-Website oder OneDrive in einem neuen InPrivate-Fenster zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="f2015-112">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>