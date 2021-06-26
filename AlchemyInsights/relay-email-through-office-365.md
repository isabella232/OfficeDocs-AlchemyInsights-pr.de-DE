---
title: Weiterleiten von E-Mails über Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117982"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="73072-102">Einrichten eines Multifunktionsgeräts oder einer Anwendung zum Senden von E-Mails</span><span class="sxs-lookup"><span data-stu-id="73072-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="73072-103">Weitere Informationen zu den verfügbaren Optionen und erforderlichen Schritten finden Sie unter [Einrichten eines Multifunktionsgeräts oder einer Anwendung zum Senden von E-Mails mithilfe von Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="73072-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="73072-104">Wenn Sie ein Gerät oder eine Anwendung haben, das/die seit Kurzem nicht mehr funktioniert, sind die häufigsten Probleme:</span><span class="sxs-lookup"><span data-stu-id="73072-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="73072-105">**Authentifizierungsbezogene Fehler bei der Verwendung der SMTP-Authentifizierungsclientübermittlung** Wir haben vor Kurzem einige Änderungen an der Funktionsweise der SMTP-Authentifizierung vorgenommen.</span><span class="sxs-lookup"><span data-stu-id="73072-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="73072-106">Weitere Informationen zum Beheben von Problemen finden Sie im Abschnitt "Authentifizierung nicht erfolgreich" unter [Beheben von Problemen mit Druckern, Scannern und Branchenanwendungen, die E-Mails mit Microsoft 365 oder Office 365 senden](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span><span class="sxs-lookup"><span data-stu-id="73072-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="73072-107">**Wir akzeptieren nur die TLS 1.2-Version, während eine sichere Verbindung zu Office 365 hergestellt wird** Wenn Sie eine sichere Verbindung (TLS) verwenden, stellen Sie sicher, dass Ihr Anwendungsgerät TLS 1.2 unterstützt.</span><span class="sxs-lookup"><span data-stu-id="73072-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="73072-108">Weitere Informationen finden Sie unter [Vorbereiten für TLS 1.2 in Office 365 und Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="73072-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="73072-109">Weitere Probleme und Lösungen finden Sie unter [Beheben von Problemen mit Druckern, Scannern und Branchenanwendungen, die E-Mails mithilfe von Microsoft 365 oder Office 365 senden](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span><span class="sxs-lookup"><span data-stu-id="73072-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="73072-110">Um betroffene Geräte anzuzeigen, wechseln Sie zum [SMTP Auth-Clientsbericht](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="73072-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="73072-p103">**Hinweis**: Exchange Online unterstützt keine Massensendungsszenarien. Um kommerzielle Massen-E-Mails (z. B. Kunden-Newsletter) zu versenden, sollten Sie Drittanbieter verwenden, die auf diese Dienste spezialisiert sind.</span><span class="sxs-lookup"><span data-stu-id="73072-p103">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios. To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
