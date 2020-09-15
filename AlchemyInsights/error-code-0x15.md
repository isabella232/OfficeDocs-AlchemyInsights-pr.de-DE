---
title: Fehler Code 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Wenn beim Aktivieren von Office 2013 für Remote Desktop Dienste (RDS)-Bereitstellungen ein Fehler auftritt, sollten Sie Adal durch Bearbeiten der Registrierung aktivieren.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709186"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Fehler bei Aktivierung Office 2013 für Remote Desktop Dienste

Wenn beim Aktivieren von Office 2013 für Remote Desktop Dienste (RDS)-Bereitstellungen ein Fehler auftritt, sollten Sie Adal durch Bearbeiten der Registrierung aktivieren.
  
|**Registrierungsschlüssel**|**Type**|**Wert**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \software\microsoft\office\15.0\common\identity\enableadal  <br/> |REG_DWORD  <br/> |1   <br/> |

Weitere Informationen finden Sie unter [Aktivieren der modernen Authentifizierung für Office 2013 auf Windows-Geräten](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  Adal ist in Microsoft 365 apps for Enterprise und Office 2016 standardmäßig aktiviert. Remote Desktop Dienste (RDS) hießen zuvor Terminal Dienste.
  