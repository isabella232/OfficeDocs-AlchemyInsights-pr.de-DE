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
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Veraltete IP-Adressbereiche für ausgehende EoP

Es wurde ein potenzielles Problem mit Ihrer Organisation festgestellt, das (falls nicht behoben durch den 26. Oktober 2018) möglicherweise den e-Mail-Fluss an Ihre lokalen oder externen Ziele unterbrechen kann. Wie bereits kommuniziert, wird zur Vereinfachung der Verwaltung von IP-Adressbereichen die IP-Adressbereiche von Exchange Online Protection (EoP) konsolidiert, die zum Senden und empfangen von e-Mails außerhalb von Office 365 verwendet werden. Unsere Analyse gibt an, dass eine oder mehrere der externen e-Mail-Quellen oder-Ziele, die Sie in Nachrichtenfluss-Konnektoren konfiguriert haben, keine Verbindungen von den [hier](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)gezeigten IP-Adressbereichen annehmen.

Handeln Sie vor dem 26. Oktober, um sicherzustellen, dass diese Quellen und Ziele Verbindungen zu und von allen [veröffentlichten EoP-IP-Adressen](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)annehmen können.

Weitere Informationen zu dieser Änderung finden Sie unter Message Center Posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)oder [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Hinweis**: Wenn Sie zuvor IP-oder URL-Veröffentlichung via HTML, XML und RSS für Endpoint-Updates verwendet haben, sollten Sie auch zu den neuen Webdiensten migrieren, um diese Arten von Updates zu automatisieren. Weitere Informationen finden Sie unter [Office 365-Endpunkt Kategorien und Office 365 IP-Adresse und URL-Webdienst](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
