---
title: Mehrere aktive Sitzungen mit demselben Postfach
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1836"
- "9000248"
ms.openlocfilehash: f4ae5c5afef9972ad4ffe74144d702ed58b2f437
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769722"
---
# <a name="multiple-active-sessions-to-the-same-mailbox"></a><span data-ttu-id="e005d-102">Mehrere aktive Sitzungen mit demselben Postfach</span><span class="sxs-lookup"><span data-stu-id="e005d-102">Multiple active sessions to the same mailbox</span></span>

<span data-ttu-id="e005d-103">Um die Verwendung von Exchange-Ressourcen zu kontrollieren, besitzt ein Postfach ein „Budget“.</span><span class="sxs-lookup"><span data-stu-id="e005d-103">To control usage of Exchange resources, a mailbox has a "budget."</span></span>

<span data-ttu-id="e005d-104">Die Ausnahme für die Überschreitung des Budgets kann von den folgenden Umstände ausgelöst werden, ist aber nicht darauf beschränkt:</span><span class="sxs-lookup"><span data-stu-id="e005d-104">The over-budget exception can be triggered by, but is not limited to, the following circumstances:</span></span>

- <span data-ttu-id="e005d-105">Einige Browserregisterkarten sind innerhalb derselben Outlook Web App-Sitzung geöffnet.</span><span class="sxs-lookup"><span data-stu-id="e005d-105">A few browser tabs are opened within the same Outlook Web App session.</span></span>

- <span data-ttu-id="e005d-106">Einige aktive Outlook Web App-Sitzungen mit demselben Postfach bestehen.</span><span class="sxs-lookup"><span data-stu-id="e005d-106">A few active Outlook Web App sessions to the same mailbox.</span></span>

- <span data-ttu-id="e005d-107">Einige andere Clientanwendungen (Outlook, Outlook Mobile, eine Drittanbieter-Clientanwendung) greifen gleichzeitig auf das Postfach zu.</span><span class="sxs-lookup"><span data-stu-id="e005d-107">A few other client applications (Outlook, Outlook Mobile, a third party client app) access the mailbox at the same time.</span></span>

- <span data-ttu-id="e005d-108">Lange andauernde Vorgänge, z. B. das Ausführen von Suchanfragen, werden aus einer anderen aktiven Postfachsitzung ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="e005d-108">Long running operations, such as executing search requests, are performed from another active mailbox session.</span></span>

