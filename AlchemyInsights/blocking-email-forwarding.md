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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219854"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blockieren oder Aufheben der Blockierung der e-Mail-Weiterleitung

Informationen zum Aktivieren oder Deaktivieren der e-Mail-Weiterleitung für ein bestimmtes Postfach finden Sie unter [Configure Email Forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Auf der Mandantenebene erfolgt die Steuerung der externen Weiterleitung mithilfe der ausgehenden Anti-Spam-Richtlinie. Wenn er auf "aus" oder "automatisch" festgelegt ist, kann die e-Mail-Weiterleitung mit dem Fehler "550 5.7.520-Zugriff verweigert, Ihre Organisation lässt keine externe Weiterleitung zulässt" blockiert werden. Wenn die Weiterleitung als blockiert festgelegt wurde, wird der Fehler angezeigt, den die Benutzer sehen.

Wenn die Weiterleitung blockiert wird, stellen Sie sicher, dass die Richtlinie für die Aktivierung von externem Autoforward konfiguriert ist. Sie können die Richtlinie für ausgehende Spam Filter über Security and Compliance Center oder durch Ausführen des Befehls Get-HostedOutboundSpamFilterPolicy | FL Name, AutoForwardingMode. Wenn Sie die Autoforward-Blockierung einrichten möchten, wird Ihnen derselbe Befehl den Status der Richtlinie jetzt mitteilen.

Hinweis: Es wird empfohlen, den externen Autoforward für die standardmäßige Richtlinie für ausgehende Spam Filter deaktiviert zu halten und nur für die Benutzer zu aktivieren, die eine externe Weiterleitung benötigen, indem Sie eine benutzerdefinierte Richtlinie für diese Benutzer erstellen. Weitere Informationen finden Sie unter [Konfigurieren der externen e-Mail-Weiterleitung in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).