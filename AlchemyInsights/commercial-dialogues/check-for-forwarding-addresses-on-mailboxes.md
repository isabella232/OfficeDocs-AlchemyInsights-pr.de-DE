---
title: Überprüfen der Weiterleitung von Adressen für Postfächer
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403310"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="071b5-102">Überprüfen der Weiterleitung von Adressen für Postfächer</span><span class="sxs-lookup"><span data-stu-id="071b5-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="071b5-103">Manchmal werden die E-Mail-Nachrichten von Benutzern von Hackern an sich selbst weitergeleitet, daher prüfen wir zunächst, ob Adressen und Regeln für das Postfach weitergeleitet werden.</span><span class="sxs-lookup"><span data-stu-id="071b5-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="071b5-104">Anschließend überprüfen wir die Überwachungsprotokolle.</span><span class="sxs-lookup"><span data-stu-id="071b5-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="071b5-105">Hier erfahren Sie, wie Sie nach Weiterleitungsadressen suchen:</span><span class="sxs-lookup"><span data-stu-id="071b5-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="071b5-106">Wählen Sie **Benutzer**  >  **Aktive Benutzer aus.**</span><span class="sxs-lookup"><span data-stu-id="071b5-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="071b5-107">Wählen Sie den Benutzer aus, dessen Konto gefährdet wurde.</span><span class="sxs-lookup"><span data-stu-id="071b5-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="071b5-108">Erweitern Sie im angezeigten Flyout die **E-Mail-Einstellungen,** und klicken Sie dann auf **Bearbeiten** für **E-Mail-Weiterleitung.**</span><span class="sxs-lookup"><span data-stu-id="071b5-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="071b5-109">Entfernen Sie alle Weiterleitungsadressen, die Sie nicht erkennen.</span><span class="sxs-lookup"><span data-stu-id="071b5-109">Remove any forwarding addresses you don't recognize.</span></span>