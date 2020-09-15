---
title: Erstellen einer e-Mail catch all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712985"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="9bfcd-102">Erstellen einer e-Mail catch all</span><span class="sxs-lookup"><span data-stu-id="9bfcd-102">Create an email catch all</span></span>

<span data-ttu-id="9bfcd-103">Für die Verwendung eines catch all wird dringend abgeraten.</span><span class="sxs-lookup"><span data-stu-id="9bfcd-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="9bfcd-104">Es ist besser, einen Bounce-Back an den Absender zu übermitteln, wenn Absender wissen, dass Ihre Nachricht nicht als adressiert zugestellt werden konnte, damit Sie Aktionen ausführen können.</span><span class="sxs-lookup"><span data-stu-id="9bfcd-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="9bfcd-105">Sie können das überwachte Postfach auch so einschränken, dass nur frühere gültige e-Mail-Adressen erfasst werden.</span><span class="sxs-lookup"><span data-stu-id="9bfcd-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="9bfcd-106">Alle Catch-Postfächer werden viel Spam erhalten und können eventuell gefüllt werden, wenn Sie nicht genau überwacht werden.</span><span class="sxs-lookup"><span data-stu-id="9bfcd-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="9bfcd-107">(Es gibt Empfangs Grenzwerte.)</span><span class="sxs-lookup"><span data-stu-id="9bfcd-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="9bfcd-108">Wenn Sie den Vorgang fortsetzen möchten, führen Sie die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="9bfcd-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="9bfcd-109">Erstellen Sie eine dynamische Verteilergruppe & "alle Empfängertypen einschließen".</span><span class="sxs-lookup"><span data-stu-id="9bfcd-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="9bfcd-110">Erstellen Sie ein dediziertes Postfach zum Abfangen von e-Mails, beispielsweise CatchAll@Domain.com.</span><span class="sxs-lookup"><span data-stu-id="9bfcd-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="9bfcd-111">Legen Sie für die spezifische Domäne den DomainType auf "InternalRelay" fest.</span><span class="sxs-lookup"><span data-stu-id="9bfcd-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="9bfcd-112">Wenn Sie später den catch all entfernen, müssen Sie die Domäne wieder auf autorisierend festlegen.</span><span class="sxs-lookup"><span data-stu-id="9bfcd-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="9bfcd-113">Erstellen Sie wie folgt eine Mailflow-Transport Regel:</span><span class="sxs-lookup"><span data-stu-id="9bfcd-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="9bfcd-114">Wenn der Absender "außerhalb der Organisation" ist</span><span class="sxs-lookup"><span data-stu-id="9bfcd-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="9bfcd-115">Umleiten der Nachricht an CatchAll@Domain.com</span><span class="sxs-lookup"><span data-stu-id="9bfcd-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="9bfcd-116">Außer wenn der Empfänger Mitglied von ALLUSERS@Domain.com ist (Verteilergruppe enthält alle Mitglieder)</span><span class="sxs-lookup"><span data-stu-id="9bfcd-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="9bfcd-117">Sicherstellen, dass überprüft wird, ob neue Postfächer der dynamischen Verteilergruppe hinzugefügt werden</span><span class="sxs-lookup"><span data-stu-id="9bfcd-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
