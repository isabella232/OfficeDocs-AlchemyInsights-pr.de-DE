---
title: 726 Blockieren der E-Mail-Weiterleitung
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059631"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blockieren oder Aufheben der E-Mail-Weiterleitung

Informationen zum Aktivieren oder Deaktivieren der E-Mail-Weiterleitung für ein bestimmtes Postfach finden Sie unter Konfigurieren der [E-Mail-Weiterleitung.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Auf Mandantenebene erfolgt die Steuerung der externen Weiterleitung mithilfe der Richtlinie für ausgehende Spamnachrichten. Sie können die Richtlinie für ausgehende Spamfilter im Security and Compliance Center [hier](https://protection.office.com/antispam) oder mit dem [Befehl "Get-HostedOutboundSpamFilterPolicy"](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)überprüfen.

Wenn Sie den folgenden Fehler erhalten: **"550 5.7.520 Zugriff verweigert, Ihre Organisation lässt keine externe Weiterleitung zu"**, stellen Sie sicher, dass die Richtlinie so konfiguriert ist, dass die externe automatische Weiterleitung aktiviert wird.

**Hinweis:** Es wird empfohlen, die externe AutoForward-Richtlinie für Ihre standardmäßige Richtlinie für ausgehende Spamfilter deaktiviert zu lassen und sie nur für die Benutzer zu aktivieren, die externe Weiterleitung benötigen, indem Sie eine benutzerdefinierte Richtlinie für diese Benutzer erstellen. Weitere Informationen finden Sie unter [Konfigurieren der externen E-Mail-Weiterleitung in Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)