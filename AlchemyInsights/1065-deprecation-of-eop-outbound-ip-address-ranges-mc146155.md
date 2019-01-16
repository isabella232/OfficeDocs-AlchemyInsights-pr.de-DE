---
title: 1065 das Verwerfen von EOP ausgehende IP-Adresse rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: ec87141ffaa2fa3484620a9b52851e3e92f20b6b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28289461"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Das Verwerfen von EOP ausgehende IP-Adressbereiche

Wir haben ein Problem mit Ihrer Organisation erkannt, die e-Mail-Fluss (sofern nicht vom 26. Oktober 2018 korrigiert) zu Ihrem lokalen oder externe Ziele auswirken kann. Zuvor mitgeteilt werden sind zur Vereinfachung der IP-Adresse Bereich Verwaltung wir die Exchange Online Protection (EOP) IP-Adressbereiche konsolidieren, die zum Senden und Empfangen von e-Mail außerhalb von Office 365 verwendet werden. Unsere Analysen weisen darauf hin, dass eine oder mehrere der externen e-Mail-Quellen oder Ziele, die Sie in der e-Mail-Fluss Connectors konfiguriert haben Verbindungen von der IP-Adressbereiche dargestellt [hier](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)akzeptiert werden nicht.
  
Vor dem 26. Oktober, um sicherzustellen, dass diese Quellen und Ziele Verbindungen zwischen allen [EOP-IP-Adressen veröffentlicht](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)akzeptiert fungieren.
  
Weitere Informationen zu dieser Änderung finden Sie unter, dass Nachrichtencenter [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)oder [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)zurücksendet.
  
 **Hinweis**: Wenn Sie zuvor IP-Adresse oder URL Veröffentlichung über HTML, XML und RSS-Endpunkt Updates verwendet, Sie auch sollte Migrieren der neuen Webdienste für diese Arten von Updates zu automatisieren. Weitere Informationen finden Sie unter [Office 365 Endpunkt Kategorien und Office 365-IP-Adresse und URL-Webdienst](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
  

