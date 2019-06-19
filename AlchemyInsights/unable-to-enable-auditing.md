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
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="7fae9-102">Die vereinheitlichte Überwachung kann nicht aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="7fae9-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="7fae9-103">Wenn Sie versuchen, die vereinheitlichte Überwachung für Ihre Office 365 Organisation zu aktivieren, erhalten Sie möglicherweise eine ähnliche Fehlermeldung wie die folgende:</span><span class="sxs-lookup"><span data-stu-id="7fae9-103">When you try to enable unified auditing for your Office 365 organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="7fae9-104">Führen Sie die folgenden Schritte aus, um dieses Problem zu beheben:</span><span class="sxs-lookup"><span data-stu-id="7fae9-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="7fae9-105">Stellen [Sie eine Verbindung mit Exchange Online PowerShell her](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="7fae9-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="7fae9-106">Führen Sie das folgende Cmdlet aus:</span><span class="sxs-lookup"><span data-stu-id="7fae9-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="7fae9-107">Warten Sie auf 60 Minuten, bis die vorherige Einstellung wirksam wird.</span><span class="sxs-lookup"><span data-stu-id="7fae9-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="7fae9-108">Führen Sie den folgenden Befehl in Exchange Online PowerShell aus:</span><span class="sxs-lookup"><span data-stu-id="7fae9-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="7fae9-109">Weitere Informationen finden Sie in den folgenden Artikeln:</span><span class="sxs-lookup"><span data-stu-id="7fae9-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="7fae9-110">Verbinden mit Exchange Online PowerShell per mehrstufiger Authentifizierung</span><span class="sxs-lookup"><span data-stu-id="7fae9-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="7fae9-111">Aktivieren oder Deaktivieren der Office 365-Überwachungsprotokollsuche</span><span class="sxs-lookup"><span data-stu-id="7fae9-111">Turn Office 365 audit log search on or off</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
