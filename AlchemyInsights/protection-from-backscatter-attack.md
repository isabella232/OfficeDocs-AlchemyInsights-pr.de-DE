---
title: Schutz vor Backscatter-Angriffen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897707"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="f07ec-102">Schutz vor Backscatter-Angriffen</span><span class="sxs-lookup"><span data-stu-id="f07ec-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="f07ec-103">Backscatter sind Nichtzustellungsberichte (auch als NDRs oder Bounce-Nachrichten bezeichnet), die Sie für Nachrichten erhalten, die Sie nicht gesendet haben.</span><span class="sxs-lookup"><span data-stu-id="f07ec-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="f07ec-104">Spammer fälschen (spoofen) die **Absender**-Adresse ihrer Nachrichten und verwenden häufig echte E-Mail-Adressen, um ihren Nachrichten Glaubwürdigkeit zu verleihen.</span><span class="sxs-lookup"><span data-stu-id="f07ec-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="f07ec-105">Wenn Spammer unweigerlich Nachrichten an nicht vorhandene Empfänger senden, wird der Ziel-E-Mail-Server im Wesentlichen dazu verleitet, die nicht zustellbare Nachricht in einem NDR an den gefälschten Absender in der **Absender:**-Adresse zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="f07ec-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="f07ec-106">Weitere Informationen finden Sie in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span><span class="sxs-lookup"><span data-stu-id="f07ec-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="f07ec-107">**Aktivieren des Backscatter-Schutzes**</span><span class="sxs-lookup"><span data-stu-id="f07ec-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="f07ec-108">Folgen Sie dem folgenden Pfad, um den Backscatter-Schutz zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="f07ec-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="f07ec-109">**protected.office.com > Bedrohungsmanagement > Richtlinie > Antispam > Wählen Sie die Spamfilterrichtlinie aus und bearbeiten Sie die Richtlinie > Spam-Eigenschaften > Als Spam markieren > NDR-Backscatter > Schalten Sie diese auf "Ein"**.</span><span class="sxs-lookup"><span data-stu-id="f07ec-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="f07ec-110">Wenn Sie der Meinung sind, dass ein Konto kompromittiert wurde, lesen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="f07ec-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="f07ec-111">Auf ein kompromittiertes E-Mail-Konto reagieren</span><span class="sxs-lookup"><span data-stu-id="f07ec-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="f07ec-112">Entfernen blockierter Benutzer aus dem Portal "Eingeschränkte Benutzer" in Office 365</span><span class="sxs-lookup"><span data-stu-id="f07ec-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



