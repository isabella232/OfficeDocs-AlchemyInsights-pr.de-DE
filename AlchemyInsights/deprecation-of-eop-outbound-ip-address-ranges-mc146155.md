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
ms.openlocfilehash: 17beb1722142d94ea05b67ce5ed1f20f8b11375c
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404820"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>VerAltete EOP-ausgehende IP-Adressbereiche

Wir haben ein potenzielles Problem mit Ihrer Organisation erkannt, das (falls nicht vom 26. Oktober 2018 korrigiert) den Nachrichtenfluss zu Ihren lokalen oder externen Zielen unterbrechen kann. Wie bereits kommuniziert, werden zur Vereinfachung der Verwaltung von IP-Adressbereichen die IP-Adressbereiche von Exchange Online Protection (EOP) konsolidiert, die zum Senden und empfangen von e-Mails außerhalb von Office 365 verwendet werden. Unsere Analyse weist darauf hin, dass eine oder mehrere externe e-Mail-Quellen oder-Ziele, die Sie in Nachrichtenübermittlungs-Konnektoren konfiguriert haben, keine Verbindungen von den [hier](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)geZEIGTEN IP-Adressbereichen annehmen.

Handeln Sie vor dem 26. Oktober, um sicherzustellen, dass diese Quellen und Ziele Verbindungen zu und von allen [veröffentlichten EoP-IP-Adressen](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)annehmen.

Weitere Informationen zu dieser Änderung finden Sie unter Nachrichten Center Beiträge [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)oder [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Hinweis**: Wenn Sie zuvor IP-oder URL-Veröffentlichung über HTML, XML und RSS für Endpunkt Aktualisierungen verwendet haben, sollten Sie auch zu den neuen Webdiensten migrieren, um diese Art von Updates zu automatisieren. Weitere Informationen finden Sie unter [office 365-Endpunkt Kategorien und office 365-IP-Adress-und-URL-Webdienst](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
