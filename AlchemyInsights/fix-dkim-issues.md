---
title: Beheben von Problemen mit DKIM-Setup
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506773"
---
# <a name="fix-dkim-setup-issues"></a>Beheben von Problemen mit DKIM-Setup

Wenn bei der Aktivierung von DKIM für Ihre benutzerdefinierte Domäne Probleme auftreten, führen Sie die folgenden Schritte aus:

- Die meisten DKIM-Setup Probleme beziehen sich auf falsche DNS-Einträge. Überprüfen Sie, ob der DKIM-CNAME-Eintrag (**kein** TXT-Eintrag) ordnungsgemäß formatiert ist. Weitere Informationen finden Sie in diesem [Thema](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Nachdem Sie Ihre DKIM-DNS-Einträge beim DNS-Hostingdienst für Ihre Domäne (in der Regel Ihre Domänenregistrierungsstelle) erstellt oder aktualisiert haben, warten Sie, bis die DNS-Einträge weitergegeben werden.

- Wenn Sie die DKIM-DNS-Einträge nicht im Admin Center erstellen können, können Sie \<CustomDomain\> durch Ihre benutzerdefinierte Domäne ersetzen (beispielsweise contoso.com) und diesen Befehl in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): Ausführen `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
