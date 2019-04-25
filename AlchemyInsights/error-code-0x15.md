---
title: Fehler Code 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Wenn beim Aktivieren von Office 2013 in Remote Desktop Dienste-Bereitstellungen eine Fehlermeldung angezeigt wird, sollten Sie die Aktivierung von ADAL durch Bearbeiten der Registrierung erwägen.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402738"
---
Wenn beim Aktivieren von Office 2013 in Remote Desktop Dienste-Bereitstellungen eine Fehlermeldung angezeigt wird, sollten Sie die Aktivierung von ADAL durch Bearbeiten der Registrierung erwägen. 
  
|**Registrierungsschlüssel**|**Typ**|**Wert**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1   <br/> |
   
Weitere Informationen finden Sie unter [Aktivieren der modernen Authentifizierung für Office 2013 auf Windows-Geräten](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL ist in Office 365 proPlus und Office 2016 standardmäßig aktiviert. > Remote Desktop Dienste (RDS) wurde zuvor als Terminal Dienste bezeichnet. 
  

