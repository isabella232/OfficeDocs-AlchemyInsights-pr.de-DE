---
title: 1554 Winsock-Fehler 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698861"
---
# <a name="winsock-error-10061"></a>Winsock-Fehler 10061

Dieser Fehlercode bedeutet, dass Microsoft keinen TCP-Socket (Connection) mit dem Ziel-Host einrichten konnte. Die wahrscheinlichste Ursache dieses Fehlers ist ein Problem mit der Konfiguration Ihrer Firewall. Um das Problem zu beheben, überprüfen Sie die folgenden Einstellungen:

- Überprüfen der Firewall-Konfiguration mit den Informationen in [Microsoft 365-URLs und IP-Adressbereichen](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Wenn der Fehler spezifisch für Exchange Online Protection (EoP) ist, sollten Sie zuvor eine Änderung an den [IP-Adressen des Exchange Online Schutzes](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)mitgeteilt haben.

- Stellen Sie sicher, dass der Internetdienstanbieter den Port nicht blockiert.

- Überprüfen Sie die Einstellungen für Smart Host und Zielserver in ihren Connectors.

Beachten Sie, dass Microsoft 365 *eingehende* Verbindungen auf diese Weise nicht blockiert.
