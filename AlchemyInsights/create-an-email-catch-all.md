---
title: Erstellen einer E-Mail-Catch-Nachricht
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816199"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="54e83-102">Erstellen einer E-Mail-Catch-Nachricht</span><span class="sxs-lookup"><span data-stu-id="54e83-102">Create an email catch all</span></span>

<span data-ttu-id="54e83-103">Die Verwendung eines catch all wird dringend abgeraten.</span><span class="sxs-lookup"><span data-stu-id="54e83-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="54e83-104">Es ist besser, eine Unzustellbarkeit an den Absender zu senden, damit Absender wissen, dass ihre Nachricht nicht als adressiert zugestellt werden konnte, damit sie Maßnahmen ergreifen können.</span><span class="sxs-lookup"><span data-stu-id="54e83-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="54e83-105">Sie können das überwachte Postfach auch darauf beschränken, nur zuvor gültige E-Mail-Adressen zu fangen.</span><span class="sxs-lookup"><span data-stu-id="54e83-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="54e83-106">Jedes Catch-All-Postfach erhält eine menge Spam und kann schließlich füllen, wenn es nicht genau überwacht wird.</span><span class="sxs-lookup"><span data-stu-id="54e83-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="54e83-107">(Es gibt Empfangsgrenzwerte.)</span><span class="sxs-lookup"><span data-stu-id="54e83-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="54e83-108">Wenn Sie den Vorgang fortsetzen möchten, führen Sie die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="54e83-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="54e83-109">Erstellen einer dynamischen Verteilergruppe & "Alle Empfängertypen" enthalten.</span><span class="sxs-lookup"><span data-stu-id="54e83-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="54e83-110">Erstellen Sie ein dediziertes Postfach zum Abfangen von E-Mails, z. B. catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="54e83-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="54e83-111">Legen Sie für die spezifische Domäne domainType auf "InternalRelay" festgelegt.</span><span class="sxs-lookup"><span data-stu-id="54e83-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="54e83-112">Wenn Sie später die catch all entfernen, stellen Sie sicher, dass die Domäne wieder auf Autoritative festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="54e83-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="54e83-113">Erstellen Sie eine Mailflow-Transportregel wie folgt:</span><span class="sxs-lookup"><span data-stu-id="54e83-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="54e83-114">Wenn der Absender "Außerhalb der Organisation" ist</span><span class="sxs-lookup"><span data-stu-id="54e83-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="54e83-115">Umleiten der Nachricht an Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="54e83-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="54e83-116">Es sei denn, der Empfänger ist Mitglied allusers@domain.com (Verteilergruppe enthält alle Mitglieder)</span><span class="sxs-lookup"><span data-stu-id="54e83-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="54e83-117">Sicherstellen, dass der dynamischen Verteilergruppe neue Postfächer hinzugefügt werden</span><span class="sxs-lookup"><span data-stu-id="54e83-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
