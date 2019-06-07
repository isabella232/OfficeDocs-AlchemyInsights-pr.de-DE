---
title: Beheben von Problemen mit DKIM-Setup
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765065"
---
# <a name="fix-dkim-setup-issues"></a>Beheben von Problemen mit DKIM-Setup

Wenn bei der Aktivierung von DKIM für Ihre benutzerdefinierte Domäne Probleme auftreten, führen Sie die folgenden Schritte aus:

- Die meisten DKIM-Setup Probleme beziehen sich auf falsche DNS-Einträge. Überprüfen Sie, ob der DKIM-CNAME-Eintrag (**kein** TXT-Eintrag) ordnungsgemäß formatiert ist. Weitere Informationen finden Sie in diesem [Thema](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Nachdem Sie Ihre DKIM-DNS-Einträge beim DNS-Hostingdienst für Ihre Domäne (in der Regel Ihre Domänenregistrierungsstelle) erstellt oder aktualisiert haben, warten Sie, bis die DNS-Einträge weitergegeben werden.

- Wenn Sie die DKIM-DNS-Einträge nicht im Admin Center erstellen können, können \<Sie\> CustomDomain durch Ihre benutzerdefinierte Domäne ersetzen (beispielsweise contoso.com) und diesen Befehl in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`ausführen.
