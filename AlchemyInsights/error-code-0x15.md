---
title: Fehlercode 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Fehler beim Aktivieren von Office 2013 auf Remote Desktop Services (RDS) Bereitstellungen empfangen werden, sollten Sie ADAL durch Bearbeiten der Registrierung aktivieren.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28289620"
---
Fehler beim Aktivieren von Office 2013 auf Remote Desktop Services (RDS) Bereitstellungen empfangen werden, sollten Sie ADAL durch Bearbeiten der Registrierung aktivieren. 
  
|**Registrierungsschlüssel**|**Typ**|**Wert**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
Weitere Informationen finden Sie unter [Modernen Authentifizierung für Office 2013 auf Windows-Geräten aktivieren](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL ist in Office 365 ProPlus und Office 2016 standardmäßig aktiviert. > Remote Desktop Services (RDS) wurde zuvor Terminaldienste bezeichnet. 
  

