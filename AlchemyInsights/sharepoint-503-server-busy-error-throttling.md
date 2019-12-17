---
title: Einschränkungen in SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 5fdbb315698a58145e5437b0a7b127ce0062a76f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048615"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="694c3-102">Einschränkungen in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="694c3-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="694c3-103">Bei dem Versuch, zu SharePoint-oder OneDrive-Websites zu navigieren, erhalten Benutzer möglicherweise einen Fehler "503 Server ist ausgelastet".</span><span class="sxs-lookup"><span data-stu-id="694c3-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="694c3-104">Dieser Fehler kann durch Drosselung im SharePoint-Dienst verursacht werden.</span><span class="sxs-lookup"><span data-stu-id="694c3-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="694c3-105">SharePoint Online verwendet Einschränkung, um eine optimale Leistung und Zuverlässigkeit des Diensts SharePoint Online verwalten.</span><span class="sxs-lookup"><span data-stu-id="694c3-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="694c3-106">Einschränkungsgrenzwerte Ruft die Anzahl von Aktionen eines Benutzers oder gleichzeitige (von Code- oder Skriptblock), um Ressourcen zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="694c3-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="694c3-107">Wenn Sie die Schritte aus gedrosselt erhalten möchten, 99 % der Zeit aufgrund von benutzerdefiniertem Code ist.</span><span class="sxs-lookup"><span data-stu-id="694c3-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="694c3-108">Weitere Informationen zur Drosselung finden Sie unter vermeiden Sie eine [Drosselung oder Blockierung in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="694c3-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="694c3-109">Wenn Sie der Meinung sind, dass dieser Fehler nicht mit der Einschränkung zusammenhängt, können Sie überprüfen, ob eine aktive Wartung auf Ihrem Mandanten erfolgt, indem Sie zum [Nachrichtencenter](https://portal.office.com/adminportal/home#/MessageCenter)navigieren.</span><span class="sxs-lookup"><span data-stu-id="694c3-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="694c3-110">Vergewissern Sie sich schließlich, dass Sie die Seite [Dienst Integrität](https://portal.office.com/adminportal/home#/servicehealth) besuchen, um nach eventuell auftretenden Warnungen/Vorfällen zu suchen.</span><span class="sxs-lookup"><span data-stu-id="694c3-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

