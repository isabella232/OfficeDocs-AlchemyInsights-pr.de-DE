---
title: SharePoint Online Drosselung
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773846"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="6b594-102">SharePoint Online Drosselung</span><span class="sxs-lookup"><span data-stu-id="6b594-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="6b594-103">**Wichtig**: Während dieser beispiellosen Zeiten unternehmen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online und OneDrive-Dienste weiterhin in hohem Ausmaß verfügbar bleiben – Bitte besuchen Sie [SharePoint Online – Temporäre Feature-Anpassungen](https://aka.ms/ODSPAdjustments), um weitere Informationen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="6b594-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="6b594-104">**503 Server ist besetzt (Fehler)**</span><span class="sxs-lookup"><span data-stu-id="6b594-104">**503 server is busy error**</span></span>

<span data-ttu-id="6b594-105">Bei dem Versuch, zu SharePoint-oder OneDrive-Websites zu navigieren, erhalten Benutzer möglicherweise einen Fehler "503 Server ist ausgelastet".</span><span class="sxs-lookup"><span data-stu-id="6b594-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="6b594-106">Dieser Fehler kann durch Drosselung im SharePoint-Dienst verursacht werden.</span><span class="sxs-lookup"><span data-stu-id="6b594-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="6b594-107">SharePoint Online verwendet Einschränkung, um eine optimale Leistung und Zuverlässigkeit des Diensts SharePoint Online verwalten.</span><span class="sxs-lookup"><span data-stu-id="6b594-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="6b594-108">Drosselung schränkt die Anzahl von Benutzeraktionen oder gleichzeitige Aufrufe (durch Code oder Skripts), um die Überlastung von Ressourcen zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="6b594-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="6b594-109">Weitere Informationen zur Drosselung finden Sie unter vermeiden Sie eine [Drosselung oder Blockierung in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="6b594-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="6b594-110">Wenn Sie der Meinung sind, dass dieser Fehler nicht mit der Einschränkung zusammenhängt, können Sie überprüfen, ob eine aktive Wartung auf Ihrem Mandanten erfolgt, indem Sie zum [Nachrichtencenter](https://portal.office.com/adminportal/home#/MessageCenter)navigieren.</span><span class="sxs-lookup"><span data-stu-id="6b594-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="6b594-111">Vergewissern Sie sich schließlich, dass Sie die Seite [Dienst Integrität](https://portal.office.com/adminportal/home#/servicehealth) besuchen, um nach eventuell auftretenden Warnungen/Vorfällen zu suchen.</span><span class="sxs-lookup"><span data-stu-id="6b594-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

