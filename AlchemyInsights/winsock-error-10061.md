---
title: 1554 Winsock-Fehler 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7651effc43cb0c4bc2fbbe5349bb72303943f493
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/13/2019
ms.locfileid: "31859139"
---
# <a name="winsock-error-10061"></a>Winsock-Fehler 10061

Dieser Fehlercode besagt, dass Office 365 keinen TCP-Socket (Verbindung) mit dem Zielhost herstellen konnte. Die wahrscheinlichste Ursache für diesen Fehler ist ein Problem mit der Konfiguration Ihrer Firewall. Um das Problem zu beheben, überprüfen Sie die folgenden Einstellungen:

- Überprüfen der Firewall-Konfiguration mit den Informationen in [Office 365-URLs und IP-Adressbereichen](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Wenn der Fehler spezifisch für Exchange Online Protection (EOP) ist, sollten Sie zuvor eine Änderung an den [Exchange Online Protection-IP-Adressen](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)mitgeteilt haben.

- Stellen Sie sicher, dass der InternetdienstAnbieter den Anschluss nicht blockiert.

- Überprüfen Sie die Einstellungen für Smarthost und Zielserver in ihren Connectors.

Beachten Sie, dass Office 365 *eingehende* Verbindungen auf diese Weise nicht blockiert.
