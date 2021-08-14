---
title: AggregateGroupMailbox vollständiger NDR, der für E-Mails empfangen wurde, die an Microsoft 365 Gruppe gesendet wurden
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: 6655bbe9482400eeb3cfdf0b91bdc595e3d98fbff0f6d9244db8bb4dd958305e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951852"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox vollständiger NDR, der für E-Mails empfangen wurde, die an Microsoft 365 Gruppe gesendet wurden

Verwenden Sie den folgenden EXO Shell-Befehl, um eine Exchange Transportregel zum automatischen Ablegen von E-Mails zu erstellen, die an das aggregierte Gruppenpostfach gesendet werden:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Ersetzen Sie die SMTP-Adresse in **"-SentTo"** durch die SMTP-Adresse des Aggregatgruppenpostfachs in Ihrem Mandanten. Sie können die SMTP-Adresse des Aggregatgruppenpostfachs vom empfangenen NDR abrufen.



