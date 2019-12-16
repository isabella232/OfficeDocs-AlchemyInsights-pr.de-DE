---
title: Erste Schritte mit SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 285c580d69efb369fa6a60066165123e3c91b0a7
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051640"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="97599-102">Workflows in SharePoint</span><span class="sxs-lookup"><span data-stu-id="97599-102">Workflows in SharePoint</span></span>

<span data-ttu-id="97599-103">Wenn SharePoint-Workflows keine e-Mails senden, hat Ihre Organisation möglicherweise die Exchange Online Absender Grenzwerte erkannt.</span><span class="sxs-lookup"><span data-stu-id="97599-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="97599-104">Die Fehlermeldung "Workflow ist angehalten" kann auftreten, wenn Sie eines der folgenden Elemente haben:</span><span class="sxs-lookup"><span data-stu-id="97599-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="97599-105">Sie verfügen über einen Workflow in SharePoint Online, der den SharePoint 2010 oder SharePoint 2013 Workflow-Plattformtyp verwendet.</span><span class="sxs-lookup"><span data-stu-id="97599-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="97599-106">Der Workflow ist so konfiguriert, dass eine benutzerdefinierte e-Mail-Nachricht an mehr als 200 Benutzer gleichzeitig gesendet wird, mehr als 10.000 Empfänger pro Tag oder mehr als 30 Nachrichten pro Minute.</span><span class="sxs-lookup"><span data-stu-id="97599-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="97599-107">Wenn Sie den Workflow ausführen, wird die e-Mail-Nachricht nicht gesendet, und Sie werden feststellen, dass die Fehlermeldung, der interne Status auf angehalten festgelegt oder an einen Empfänger nicht gesendet werden kann, angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="97599-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="97599-108">Weitere Informationen finden Sie im folgenden [Artikel](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="97599-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

