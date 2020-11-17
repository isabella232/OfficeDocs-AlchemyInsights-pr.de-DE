---
title: Vorbereiten für die Verwendung von TLS 1.2 in Microsoft 365
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 1ec40ba36c69296298e24dca64a873d53682833a
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085903"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a><span data-ttu-id="a8973-102">Vorbereiten für die Verwendung von TLS 1.2 in Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a8973-102">Prepare for use of TLS 1.2 in Microsoft 365</span></span>

<span data-ttu-id="a8973-103">Ab dem 31. Oktober 2018 wird Microsoft 365 weiter auf TLS 1.2 umgestellt.</span><span class="sxs-lookup"><span data-stu-id="a8973-103">As of October 31st, 2018, Microsoft 365 will continue transitioning to TLS 1.2.</span></span> <span data-ttu-id="a8973-104">Ab dem 15. Oktober 2020 beginnt O365 mit der dienstweiten Einstellung von TLS 1.0 und 1.1.</span><span class="sxs-lookup"><span data-stu-id="a8973-104">Starting October 15, 2020, O365 will begin the deprecation of TLS 1.0 and 1.1 across the service.</span></span> <span data-ttu-id="a8973-105">Diese Änderung wird in den nächsten Wochen und Monaten fortgesetzt, aber die Kunden sollten davon ausgehen, dass ab dem 15. Oktober 2020 keine TLS 1.0- und TLS 1.1-Anrufe mit O365 möglich sind.</span><span class="sxs-lookup"><span data-stu-id="a8973-105">The rollout of this change will continue over the next few weeks and months, but customers should assume no TLS 1.0/1.1 calls will work when engaging with O365 starting Oct 15, 2020.</span></span> <span data-ttu-id="a8973-106">Wie bereits mitgeteilt (MC126199 im Dez. 2017, MC128929 im Feb. 2018, MC186827 im Juli 2019 und MC218794 im Juli 2020), verlagern wir alle unsere Onlinedienste in Transport Layer Security (TLS) 1.2+, um die erstklassige Verschlüsselung zu gewährleisten und sicherzustellen, dass unser Dienst standardmäßig sicherer ist.</span><span class="sxs-lookup"><span data-stu-id="a8973-106">As previously communicated (MC126199 in Dec 2017, MC128929 in Feb 2018, MC186827 in July 2019, and MC218794 in July 2020), we are moving all of our online services to Transport Layer Security (TLS) 1.2+ to provide best-in-class encryption, and to ensure our service is more secure, by default.</span></span> <span data-ttu-id="a8973-107">Kunden können weiterhin auswählen, ob sie TLS 1.0 bzw. 1.1 auf ihren Servern und Ressourcen installieren, doch sollten sie davon ausgehen, dass nur TLS 1.2 und höher funktionieren, wenn sie mit O365-Ressourcen arbeiten.</span><span class="sxs-lookup"><span data-stu-id="a8973-107">Customers can still choose to have TLS 1.0/1.1 on their servers and resources, but they should assume only TLS 1.2 or higher will work when interacting with O365 resources.</span></span>
  
<span data-ttu-id="a8973-108">Weitere Informationen zu diesen Änderungen finden Sie [hier](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) und [hier](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="a8973-108">To learn more about these changes, please see [here](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) and [here](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).</span></span>

  