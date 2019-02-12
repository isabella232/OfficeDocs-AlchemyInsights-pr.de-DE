---
title: 1065 das Verwerfen von EOP ausgehende IP-Adresse rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 2b4b2e2341f45e2d37713d72a2e0d34fa1a9a7cc
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934883"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="8e564-102">Das Verwerfen von EOP ausgehende IP-Adressbereiche</span><span class="sxs-lookup"><span data-stu-id="8e564-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="8e564-p101">Wir haben ein Problem mit Ihrer Organisation erkannt, die e-Mail-Fluss (sofern nicht vom 26. Oktober 2018 korrigiert) zu Ihrem lokalen oder externe Ziele auswirken kann. Zuvor mitgeteilt werden sind zur Vereinfachung der IP-Adresse Bereich Verwaltung wir die Exchange Online Protection (EOP) IP-Adressbereiche konsolidieren, die zum Senden und Empfangen von e-Mail außerhalb von Office 365 verwendet werden. Unsere Analysen weisen darauf hin, dass eine oder mehrere der externen e-Mail-Quellen oder Ziele, die Sie in der e-Mail-Fluss Connectors konfiguriert haben Verbindungen von der IP-Adressbereiche dargestellt [hier](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)akzeptiert werden nicht.</span><span class="sxs-lookup"><span data-stu-id="8e564-p101">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations. As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365. Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="8e564-106">Vor dem 26. Oktober, um sicherzustellen, dass diese Quellen und Ziele Verbindungen zwischen allen [EOP-IP-Adressen veröffentlicht](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)akzeptiert fungieren.</span><span class="sxs-lookup"><span data-stu-id="8e564-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="8e564-107">Weitere Informationen zu dieser Änderung finden Sie unter, dass Nachrichtencenter [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)oder [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)zurücksendet.</span><span class="sxs-lookup"><span data-stu-id="8e564-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="8e564-p102">**Hinweis**: Wenn Sie zuvor IP-Adresse oder URL Veröffentlichung über HTML, XML und RSS-Endpunkt Updates verwendet, Sie auch sollte Migrieren der neuen Webdienste für diese Arten von Updates zu automatisieren. Weitere Informationen finden Sie unter [Office 365 Endpunkt Kategorien und Office 365-IP-Adresse und URL-Webdienst](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="8e564-p102">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates. For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

