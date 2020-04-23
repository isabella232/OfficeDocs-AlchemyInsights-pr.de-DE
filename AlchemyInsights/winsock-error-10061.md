---
title: 1554 Winsock-Fehler 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766168"
---
# <a name="winsock-error-10061"></a>Winsock-Fehler 10061

Dieser Fehlercode bedeutet, dass Microsoft keinen TCP-Socket (Connection) mit dem Ziel-Host einrichten konnte. Die wahrscheinlichste Ursache dieses Fehlers ist ein Problem mit der Konfiguration Ihrer Firewall. Um das Problem zu beheben, überprüfen Sie die folgenden Einstellungen:

- Überprüfen der Firewall-Konfiguration mit den Informationen in [Microsoft 365-URLs und IP-Adressbereichen](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Wenn der Fehler spezifisch für Exchange Online Protection (EoP) ist, sollten Sie zuvor eine Änderung an den [IP-Adressen des Exchange Online Schutzes](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)mitgeteilt haben.

- Stellen Sie sicher, dass der Internetdienstanbieter den Port nicht blockiert.

- Überprüfen Sie die Einstellungen für Smart Host und Zielserver in ihren Connectors.

Beachten Sie, dass Microsoft 365 *eingehende* Verbindungen auf diese Weise nicht blockiert.
