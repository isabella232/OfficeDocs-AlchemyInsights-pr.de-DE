---
title: Aktivieren der Postfachüberwachung
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703570"
---
# <a name="enable-mailbox-auditing"></a>Aktivieren der Postfachüberwachung

Um die postfachüberwachung für einen einzelnen Benutzer oder eine gesamte Organisation zu aktivieren, müssen die folgenden Cmdlets von der Remote-Power Shell aus ausgeführt werden:
  
 **Einzelner Benutzer**
  
Festlegen-Mailbox-Identity "Jane Dow"-AuditEnabled $true
  
 **Organisation**
  
Get-Mailbox-resultse Unlimited-Filter {RecipientTypeDetails-EQ "User Mailbox"} | Festlegen-Mailbox-AuditEnabled $true
  
[Weitere Informationen](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

