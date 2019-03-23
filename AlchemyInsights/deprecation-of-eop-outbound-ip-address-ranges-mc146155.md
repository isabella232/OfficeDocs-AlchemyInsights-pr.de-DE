---
title: 1065 verAltete EOP-ausgehende IP-Adresse rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 0def0a93c61ea762918f1c9e6edb2e9b04446851
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/22/2019
ms.locfileid: "30777271"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="2950a-102">VerAltete EOP-ausgehende IP-Adressbereiche</span><span class="sxs-lookup"><span data-stu-id="2950a-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="2950a-103">Wir haben ein potenzielles Problem mit Ihrer Organisation erkannt, das (falls nicht vom 26. Oktober 2018 korrigiert) den Nachrichtenfluss zu Ihren lokalen oder externen Zielen unterbrechen kann.</span><span class="sxs-lookup"><span data-stu-id="2950a-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="2950a-104">Wie bereits kommuniziert, werden zur Vereinfachung der Verwaltung von IP-Adressbereichen die IP-Adressbereiche von Exchange Online Protection (EOP) konsolidiert, die zum Senden und empfangen von e-Mails außerhalb von Office 365 verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="2950a-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365.</span></span> <span data-ttu-id="2950a-105">Unsere Analyse weist darauf hin, dass eine oder mehrere externe e-Mail-Quellen oder-Ziele, die Sie in Nachrichtenübermittlungs-Konnektoren konfiguriert haben, keine Verbindungen von den [hier](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)geZEIGTEN IP-Adressbereichen annehmen.</span><span class="sxs-lookup"><span data-stu-id="2950a-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="2950a-106">Handeln Sie vor dem 26. Oktober, um sicherzustellen, dass diese Quellen und Ziele Verbindungen zu und von allen [veröffentlichten EoP-IP-Adressen](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)annehmen.</span><span class="sxs-lookup"><span data-stu-id="2950a-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="2950a-107">Weitere Informationen zu dieser Änderung finden Sie unter Nachrichten Center Beiträge [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)oder [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="2950a-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="2950a-108">**Hinweis**: Wenn Sie zuvor IP-oder URL-Veröffentlichung über HTML, XML und RSS für Endpunkt Aktualisierungen verwendet haben, sollten Sie auch zu den neuen Webdiensten migrieren, um diese Art von Updates zu automatisieren.</span><span class="sxs-lookup"><span data-stu-id="2950a-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="2950a-109">Weitere Informationen finden Sie unter [office 365-Endpunkt Kategorien und office 365-IP-Adress-und-URL-Webdienst](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="2950a-109">For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

