---
title: 1554 Winsock-Fehler 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: f54c7fc81c274871fbc22908ce0fb21500975d9e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530788"
---
# <a name="winsock-error-10061"></a>Winsock-Fehler 10061

Dieser Fehlercode bedeutet, dass Office 365 keinen TCP-Socket (Connection) mit dem Ziel Host einrichten konnten. Die wahrscheinlichste Ursache dieses Fehlers ist ein Problem mit der Konfiguration Ihrer Firewall. Um das Problem zu beheben, überprüfen Sie die folgenden Einstellungen:

- Überprüfen der Firewall-Konfiguration mit den Informationen in [Office 365-URLs und IP-Adressbereichen](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Wenn der Fehler spezifisch für Exchange Online Protection (EoP) ist, sollten Sie zuvor eine Änderung an den [IP-Adressen des Exchange Online Schutzes](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)mitgeteilt haben.

- Stellen Sie sicher, dass der Internetdienstanbieter den Port nicht blockiert.

- Überprüfen Sie die Einstellungen für Smart Host und Zielserver in ihren Connectors.

Beachten Sie, dass Office 365 *eingehende* Verbindungen auf diese Weise nicht blockiert.
