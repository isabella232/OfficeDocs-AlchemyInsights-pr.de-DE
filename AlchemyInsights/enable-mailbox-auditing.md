---
title: Aktivieren der Postfachüberwachung
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736252"
---
# <a name="enable-mailbox-auditing"></a>Aktivieren der Postfachüberwachung

Um die postfachüberwachung für einen einzelnen Benutzer oder eine gesamte Organisation zu aktivieren, müssen die folgenden Cmdlets von der Remote-Power Shell aus ausgeführt werden:
  
 **Einzelner Benutzer**
  
Festlegen-Mailbox-Identity "Jane Dow"-AuditEnabled $true
  
 **Organisation**
  
Get-Mailbox-resultse Unlimited-Filter {RecipientTypeDetails-EQ "User Mailbox"} | Festlegen-Mailbox-AuditEnabled $true
  
[Weitere Informationen](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

