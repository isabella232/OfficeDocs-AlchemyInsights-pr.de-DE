---
title: Fehler Code 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Wenn beim Aktivieren von Office 2013 für Remote Desktop Dienste (RDS)-Bereitstellungen ein Fehler auftritt, sollten Sie Adal durch Bearbeiten der Registrierung aktivieren.
ms.openlocfilehash: e2249d8ebbd2313c64dda5656a3243fa76d97a9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35388244"
---
Wenn beim Aktivieren von Office 2013 für Remote Desktop Dienste (RDS)-Bereitstellungen ein Fehler auftritt, sollten Sie Adal durch Bearbeiten der Registrierung aktivieren.
  
|**Registrierungsschlüssel**|**Typ**|**Wert**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Weitere Informationen finden Sie unter [Aktivieren der modernen Authentifizierung für Office 2013 auf Windows-Geräten](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  Adal ist in Office 365 ProPlus und Office 2016 standardmäßig aktiviert. Zuvor wurden #a0 Remote Desktop Dienste (RDS) als Terminal Dienste bezeichnet.
  