---
title: Weiterleiten von E-Mails über Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 180bae451941e4aaea94d285362794a797383eca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776485"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="c2ff2-102">Einrichten eines Multifunktionsgeräts oder einer Anwendung zum Senden von E-Mails</span><span class="sxs-lookup"><span data-stu-id="c2ff2-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="c2ff2-103">Weitere Informationen zu den verfügbaren Optionen und erforderlichen Schritten finden Sie unter [Einrichten eines Multifunktionsgeräts oder einer Anwendung zum Senden von E-Mails mithilfe von Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="c2ff2-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="c2ff2-104">**Hinweis:** Wenn Sie ein Gerät oder eine Anwendung nutzen, das/die seit Kurzem nicht mehr funktioniert, beachten Sie bitte, dass wir kürzlich damit begonnen haben, das [3DES-Verschlüsselungsverfahren wie geplant zu deaktivieren](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption).</span><span class="sxs-lookup"><span data-stu-id="c2ff2-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="c2ff2-105">Um betroffene Geräte anzuzeigen, wechseln Sie zum [SMTP Auth-Clientsbericht](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="c2ff2-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="c2ff2-106">Häufige Fehler können sein: Authentifizierungsfehler/Fehler, TLS-Fehler/Fehler, Verschlüsselungsalgorithmusfehler, Algorithmuskonflikt oder „Verbindung unterbrochen“.</span><span class="sxs-lookup"><span data-stu-id="c2ff2-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="c2ff2-107">So lösen Sie das Problem:</span><span class="sxs-lookup"><span data-stu-id="c2ff2-107">To resolve the issue:</span></span>

 - <span data-ttu-id="c2ff2-108">**Windows Server 2003 IIS SMTP funktioniert nicht mehr, eine neuere Version von Windows ist erforderlich.**</span><span class="sxs-lookup"><span data-stu-id="c2ff2-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="c2ff2-109">Bitte erkundigen Sie sich bei Ihrem Anwendungs- oder Gerätehersteller, ob ein modernes Verschlüsselungsverfahren unterstützt wird oder ob es ein Update gibt.</span><span class="sxs-lookup"><span data-stu-id="c2ff2-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
