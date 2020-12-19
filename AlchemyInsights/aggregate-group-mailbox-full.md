---
title: AggregateGroupMailbox vollständiger NDR für e-Mails, die an die Microsoft 365-Gruppe gesendet wurden
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
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2020
ms.locfileid: "49715698"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox vollständiger NDR für e-Mails, die an die Microsoft 365-Gruppe gesendet wurden

Verwenden Sie den folgenden Exo-Shell-Befehl, um eine Exchange-Transportregel zum automatischen ablegen von e-Mails zu erstellen, die an das Aggregat Gruppenpostfach gesendet werden:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Ersetzen Sie die SMTP-Adresse in **-SentTo** durch die SMTP-Adresse des Aggregat Gruppen Postfachs in Ihrem Mandanten. Sie können die SMTP-Adresse des Aggregat Gruppen Postfachs aus dem empfangenen Unzustellbarkeitsbericht abrufen.



