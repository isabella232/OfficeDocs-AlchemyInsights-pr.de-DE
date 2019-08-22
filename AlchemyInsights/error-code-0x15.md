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
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36526992"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Fehler bei Aktivierung Office 2013 für Remote Desktop Dienste

Wenn beim Aktivieren von Office 2013 für Remote Desktop Dienste (RDS)-Bereitstellungen ein Fehler auftritt, sollten Sie Adal durch Bearbeiten der Registrierung aktivieren.
  
|**Registrierungsschlüssel**|**Typ**|**Wert**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Weitere Informationen finden Sie unter [Aktivieren der modernen Authentifizierung für Office 2013 auf Windows-Geräten](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  Adal ist in Office 365 ProPlus und Office 2016 standardmäßig aktiviert. Remote Desktop Dienste (RDS) hießen zuvor Terminal Dienste.
  