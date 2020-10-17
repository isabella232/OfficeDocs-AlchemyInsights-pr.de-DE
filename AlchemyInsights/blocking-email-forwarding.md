---
title: 726 Blockierung der e-Mail-Weiterleitung
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
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478346"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blockieren oder Aufheben der Blockierung der e-Mail-Weiterleitung

Informationen zum Aktivieren oder Deaktivieren der e-Mail-Weiterleitung für ein bestimmtes Postfach finden Sie unter [Configure Email Forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Auf der Mandantenebene erfolgt die Steuerung der externen Weiterleitung mithilfe der ausgehenden Spam Richtlinie. Sie können die Richtlinie für ausgehende Spamfilter aus dem Security and Compliance Center [hier](https://protection.office.com/antispam) oder mithilfe des [Befehls Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)überprüfen.

Wenn Sie die folgende Fehlermeldung erhalten: **"550 5.7.520 Zugriff verweigert, Ihre Organisation lässt keine externe Weiterleitung zu"**, stellen Sie sicher, dass die Richtlinie so konfiguriert ist, dass externe automatische Weiterleitung aktiviert wird.

**Hinweis:** Es wird empfohlen, den externen Autoforward für die standardmäßige Richtlinie für ausgehende Spamfilter deaktiviert zu halten und nur für die Benutzer zu aktivieren, die eine externe Weiterleitung benötigen, indem Sie eine benutzerdefinierte Richtlinie für diese Benutzer erstellen. Weitere Informationen finden Sie unter [Konfigurieren der externen e-Mail-Weiterleitung in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).