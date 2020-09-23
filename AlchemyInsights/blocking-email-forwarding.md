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
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="13f35-102">Blockieren oder Aufheben der Blockierung der e-Mail-Weiterleitung</span><span class="sxs-lookup"><span data-stu-id="13f35-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="13f35-103">Informationen zum Aktivieren oder Deaktivieren der e-Mail-Weiterleitung für ein bestimmtes Postfach finden Sie unter [Configure Email Forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="13f35-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="13f35-104">Auf der Mandantenebene erfolgt die Steuerung der externen Weiterleitung mithilfe der ausgehenden Anti-Spam-Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="13f35-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="13f35-105">Wenn er auf "aus" oder "automatisch" festgelegt ist, kann die e-Mail-Weiterleitung mit dem Fehler "550 5.7.520-Zugriff verweigert, Ihre Organisation lässt keine externe Weiterleitung zulässt" blockiert werden.</span><span class="sxs-lookup"><span data-stu-id="13f35-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="13f35-106">Wenn die Weiterleitung als blockiert festgelegt wurde, wird der Fehler angezeigt, den die Benutzer sehen.</span><span class="sxs-lookup"><span data-stu-id="13f35-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="13f35-107">Wenn die Weiterleitung blockiert wird, stellen Sie sicher, dass die Richtlinie für die Aktivierung von externem Autoforward konfiguriert ist.</span><span class="sxs-lookup"><span data-stu-id="13f35-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="13f35-108">Sie können die Richtlinie für ausgehende Spam Filter über Security and Compliance Center oder durch Ausführen des Befehls Get-HostedOutboundSpamFilterPolicy | FL Name, AutoForwardingMode.</span><span class="sxs-lookup"><span data-stu-id="13f35-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="13f35-109">Wenn Sie die Autoforward-Blockierung einrichten möchten, wird Ihnen derselbe Befehl den Status der Richtlinie jetzt mitteilen.</span><span class="sxs-lookup"><span data-stu-id="13f35-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="13f35-110">Hinweis: Es wird empfohlen, den externen Autoforward für die standardmäßige Richtlinie für ausgehende Spam Filter deaktiviert zu halten und nur für die Benutzer zu aktivieren, die eine externe Weiterleitung benötigen, indem Sie eine benutzerdefinierte Richtlinie für diese Benutzer erstellen.</span><span class="sxs-lookup"><span data-stu-id="13f35-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="13f35-111">Weitere Informationen finden Sie unter [Konfigurieren der externen e-Mail-Weiterleitung in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="13f35-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>