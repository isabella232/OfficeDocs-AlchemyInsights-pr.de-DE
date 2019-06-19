---
title: 2419-nicht aktivierbar-Überwachung
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065641"
---
# <a name="unable-to-enable-unified-auditing"></a>Die vereinheitlichte Überwachung kann nicht aktiviert werden.

Wenn Sie versuchen, die vereinheitlichte Überwachung für Ihre Office 365 Organisation zu aktivieren, erhalten Sie möglicherweise eine ähnliche Fehlermeldung wie die folgende:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Führen Sie die folgenden Schritte aus, um dieses Problem zu beheben:

1. Stellen [Sie eine Verbindung mit Exchange Online PowerShell her](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Führen Sie das folgende Cmdlet aus:

   ```
   Enable-OrganizationCustomization
   ```

3. Warten Sie auf 60 Minuten, bis die vorherige Einstellung wirksam wird.

4. Führen Sie den folgenden Befehl in Exchange Online PowerShell aus:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Weitere Informationen finden Sie in den folgenden Artikeln:

- [Verbinden mit Exchange Online PowerShell per mehrstufiger Authentifizierung](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Aktivieren oder Deaktivieren der Office 365-Überwachungsprotokollsuche](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
