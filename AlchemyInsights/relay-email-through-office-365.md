---
title: Weiterleiten von E-Mails über Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 074a9106553bf3a2a5e563f9ebaca9dfc38111cb
ms.sourcegitcommit: 9872280f71429d2344b0b441e218fba5b3bd3cf7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/02/2020
ms.locfileid: "45023458"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="07715-102">Einrichten eines Multifunktionsgeräts oder einer Anwendung zum Senden von E-Mails</span><span class="sxs-lookup"><span data-stu-id="07715-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="07715-103">Weitere Informationen zu den verfügbaren Optionen und erforderlichen Schritten finden Sie unter [Einrichten eines Multifunktionsgeräts oder einer Anwendung zum Senden von E-Mails mithilfe von Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="07715-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="07715-104">**Hinweis:** Wenn Sie ein Gerät oder eine Anwendung nutzen, das/die seit Kurzem nicht mehr funktioniert, beachten Sie bitte, dass wir kürzlich damit begonnen haben, das [3DES-Verschlüsselungsverfahren wie geplant zu deaktivieren](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption).</span><span class="sxs-lookup"><span data-stu-id="07715-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="07715-105">Um betroffene Geräte anzuzeigen, wechseln Sie zum [SMTP Auth-Clientsbericht](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="07715-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="07715-106">Häufige Fehler können sein: Authentifizierungsfehler/Fehler, TLS-Fehler/Fehler, Verschlüsselungsalgorithmusfehler, Algorithmuskonflikt oder „Verbindung unterbrochen“.</span><span class="sxs-lookup"><span data-stu-id="07715-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="07715-107">So lösen Sie das Problem:</span><span class="sxs-lookup"><span data-stu-id="07715-107">To resolve the issue:</span></span>

 - <span data-ttu-id="07715-108">**Windows Server 2003 IIS SMTP funktioniert nicht mehr, eine neuere Version von Windows ist erforderlich.**</span><span class="sxs-lookup"><span data-stu-id="07715-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="07715-109">Bitte erkundigen Sie sich bei Ihrem Anwendungs- oder Gerätehersteller, ob ein modernes Verschlüsselungsverfahren unterstützt wird oder ob es ein Update gibt.</span><span class="sxs-lookup"><span data-stu-id="07715-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
