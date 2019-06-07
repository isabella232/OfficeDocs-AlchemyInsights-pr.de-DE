---
title: 1065 veraltete EoP der ausgehenden IP-Adresse rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 9860845dea444847833d4c5cd01d49ea93473778
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752954"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="06224-102">Veraltete IP-Adressbereiche für ausgehende EoP</span><span class="sxs-lookup"><span data-stu-id="06224-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="06224-103">Es wurde ein potenzielles Problem mit Ihrer Organisation festgestellt, das (falls nicht behoben durch den 26. Oktober 2018) möglicherweise den e-Mail-Fluss an Ihre lokalen oder externen Ziele unterbrechen kann.</span><span class="sxs-lookup"><span data-stu-id="06224-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="06224-104">Wie bereits kommuniziert, wird zur Vereinfachung der Verwaltung von IP-Adressbereichen die IP-Adressbereiche von Exchange Online Protection (EoP) konsolidiert, die zum Senden und empfangen von e-Mails außerhalb von Office 365 verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="06224-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365.</span></span> <span data-ttu-id="06224-105">Unsere Analyse gibt an, dass eine oder mehrere der externen e-Mail-Quellen oder-Ziele, die Sie in Nachrichtenfluss-Konnektoren konfiguriert haben, keine Verbindungen von den [hier](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)gezeigten IP-Adressbereichen annehmen.</span><span class="sxs-lookup"><span data-stu-id="06224-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="06224-106">Handeln Sie vor dem 26. Oktober, um sicherzustellen, dass diese Quellen und Ziele Verbindungen zu und von allen [veröffentlichten EoP-IP-Adressen](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)annehmen können.</span><span class="sxs-lookup"><span data-stu-id="06224-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="06224-107">Weitere Informationen zu dieser Änderung finden Sie unter Message Center Posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)oder [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="06224-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="06224-108">**Hinweis**: Wenn Sie zuvor IP-oder URL-Veröffentlichung via HTML, XML und RSS für Endpoint-Updates verwendet haben, sollten Sie auch zu den neuen Webdiensten migrieren, um diese Arten von Updates zu automatisieren.</span><span class="sxs-lookup"><span data-stu-id="06224-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="06224-109">Weitere Informationen finden Sie unter [Office 365-Endpunkt Kategorien und Office 365 IP-Adresse und URL-Webdienst](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="06224-109">For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
