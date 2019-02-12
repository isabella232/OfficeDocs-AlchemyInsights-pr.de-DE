---
title: 1554 10061 Winsock-Fehler
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903096"
---
# <a name="winsock-error-10061"></a>Winsock-Fehler 10061

Dieser Fehlercode bedeutet, dass einen TCP-Socket (Verbindung) mit den Zielhost ein Office 365 hergestellt werden konnte nicht. Höchstwahrscheinlich für diesen Fehler ist ein Problem mit der Konfiguration Ihrer Firewall. Um das Problem zu beheben, überprüfen Sie diese Einstellungen:
  
- Überprüfen Sie die Konfiguration Ihrer Firewall mit den Informationen in [Office 365-URLs und IP-Adressbereiche](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Wenn der Fehler bestimmte Exchange Online Protection (EOP) ist, sollten haben Sie bereits auf eine Änderung der [Exchange Online Protection-IP-Adressen](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)benachrichtigt.
    
- Stellen Sie sicher, dass Ihr Internetdienstanbieter (ISP) den Port nicht blockiert.
    
- Vergewissern Sie sich smart Host und Ziel-servereinstellungen in die Connectors.
    
Beachten Sie, dass Office 365 *eingehende* Verbindungen auf diese Weise nicht blockiert. 
  

