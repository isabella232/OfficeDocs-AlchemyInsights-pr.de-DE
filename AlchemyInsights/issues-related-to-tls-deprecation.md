---
title: E-Mails an/von Office 365 können aufgrund der TLS 1.0- und TLS 1.1-Deaktivierung nicht gesendet/empfangen werden.
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50726918"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>E-Mails an/von Office 365 können aufgrund der TLS 1.0- und TLS 1.1-Deaktivierung nicht gesendet/empfangen werden.

Wie vom Nachrichtencenter nach MC229914 bestätigt wurde, begannen die Veraltetkeit von TLS 1.0 und TLS 1.1 mit der Erzwingung für Exchange Online-Nachrichtenflussendpunkte. In Kürze akzeptiert Office 365 keine TLS 1.0- und TLS 1.1-E-Mail-Verbindungen aus externen Quellen mehr. Darüber hinaus verwendet Exchange Online niemals TLS 1.0 oder 1.1, um ausgehende E-Mails zu senden. Wenn aufgrund der TLS 1.0- oder 1.1-Deaktivierung Probleme auftreten, kann einer der folgenden Fehler auftreten:

- Absender bekommt NDR-Unzustellbarkeit zurück - "421 4.4.2 Verbindung aufgrund von SocketError gelöscht"
- Fehler in der Warteschlangenanzeige des lokalen Servers, der E-Mails an Officer 365- '421 4.4.2 Verbindung aufgrund von SocketError' sendet
- Fehler im Protokoll des [Sendeconnectorprotokolls](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) auf dem Server, der E-Mails an Office 365 sendet: Fehler bei TLS-Aushandlung mit Fehler SocketError
- Fehler im Protokoll des Sende- oder Empfangsconnectorprotokolls – '451 5.7.3 Muss zuerst einen STARTTLS-Befehl ausführen'

Wenn einer der oben genannten Fehler aufgetreten ist, stellen Sie sicher, dass auf dem Server, auf dem E-Mails gesendet oder empfangen werden, TLS 1.2 aktiviert ist, indem Sie die folgenden Registrierungsschlüssel überprüfen:

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:000000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:000000001**

Wenn Sie änderungen an den oben genannten Registrierungsschlüsseln vornehmen, um TLS 1.2 zu aktivieren, starten Sie den Server neu, damit die Änderungen wirksam werden. Stellen Sie außerdem sicher, dass Die neuesten Windows- und Exchange-Updates installiert sind.

Weitere Informationen finden Sie hier:

- [Exchange Server TLS Guidance, Teil 1: Getting Ready for TLS 1.2 - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server TLS-Leitfaden Teil 2: Aktivieren von TLS 1.2 und Identifizieren von Clients, die es nicht verwenden – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Grundlegendes zu E-Mail-Szenarien, wenn TLS-Versionen nicht mit Exchange Online vereinbart werden können – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
