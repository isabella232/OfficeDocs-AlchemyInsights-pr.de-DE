---
title: Beheben von Problemen mit DKIM-Setup
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744949"
---
# <a name="fix-dkim-setup-issues"></a>Beheben von Problemen mit DKIM-Setup

Wenn bei der Aktivierung von DKIM für Ihre benutzerdefinierte Domäne Probleme auftreten, führen Sie die folgenden Schritte aus:

- Die meisten DKIM-Setup Probleme beziehen sich auf falsche DNS-Einträge. Überprüfen Sie, ob der DKIM-CNAME-Eintrag (**kein** TXT-Eintrag) ordnungsgemäß formatiert ist. Weitere Informationen finden Sie in diesem [Thema](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Nachdem Sie Ihre DKIM-DNS-Einträge beim DNS-Hostingdienst für Ihre Domäne (in der Regel Ihre Domänenregistrierungsstelle) erstellt oder aktualisiert haben, warten Sie, bis die DNS-Einträge weitergegeben werden.

- Wenn Sie die DKIM-DNS-Einträge nicht im Admin Center erstellen können, können Sie \<CustomDomain\> durch Ihre benutzerdefinierte Domäne ersetzen (beispielsweise contoso.com) und diesen Befehl in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): Ausführen `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
