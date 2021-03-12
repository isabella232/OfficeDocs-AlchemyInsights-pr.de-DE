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
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="0d3cf-102">E-Mails an/von Office 365 können aufgrund der TLS 1.0- und TLS 1.1-Deaktivierung nicht gesendet/empfangen werden.</span><span class="sxs-lookup"><span data-stu-id="0d3cf-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="0d3cf-103">Wie vom Nachrichtencenter nach MC229914 bestätigt wurde, begannen die Veraltetkeit von TLS 1.0 und TLS 1.1 mit der Erzwingung für Exchange Online-Nachrichtenflussendpunkte.</span><span class="sxs-lookup"><span data-stu-id="0d3cf-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="0d3cf-104">In Kürze akzeptiert Office 365 keine TLS 1.0- und TLS 1.1-E-Mail-Verbindungen aus externen Quellen mehr.</span><span class="sxs-lookup"><span data-stu-id="0d3cf-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="0d3cf-105">Darüber hinaus verwendet Exchange Online niemals TLS 1.0 oder 1.1, um ausgehende E-Mails zu senden.</span><span class="sxs-lookup"><span data-stu-id="0d3cf-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="0d3cf-106">Wenn aufgrund der TLS 1.0- oder 1.1-Deaktivierung Probleme auftreten, kann einer der folgenden Fehler auftreten:</span><span class="sxs-lookup"><span data-stu-id="0d3cf-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="0d3cf-107">Absender bekommt NDR-Unzustellbarkeit zurück - "421 4.4.2 Verbindung aufgrund von SocketError gelöscht"</span><span class="sxs-lookup"><span data-stu-id="0d3cf-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="0d3cf-108">Fehler in der Warteschlangenanzeige des lokalen Servers, der E-Mails an Officer 365- '421 4.4.2 Verbindung aufgrund von SocketError' sendet</span><span class="sxs-lookup"><span data-stu-id="0d3cf-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="0d3cf-109">Fehler im Protokoll des [Sendeconnectorprotokolls](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) auf dem Server, der E-Mails an Office 365 sendet: Fehler bei TLS-Aushandlung mit Fehler SocketError</span><span class="sxs-lookup"><span data-stu-id="0d3cf-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="0d3cf-110">Fehler im Protokoll des Sende- oder Empfangsconnectorprotokolls – '451 5.7.3 Muss zuerst einen STARTTLS-Befehl ausführen'</span><span class="sxs-lookup"><span data-stu-id="0d3cf-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="0d3cf-111">Wenn einer der oben genannten Fehler aufgetreten ist, stellen Sie sicher, dass auf dem Server, auf dem E-Mails gesendet oder empfangen werden, TLS 1.2 aktiviert ist, indem Sie die folgenden Registrierungsschlüssel überprüfen:</span><span class="sxs-lookup"><span data-stu-id="0d3cf-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="0d3cf-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:000000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:000000001**</span><span class="sxs-lookup"><span data-stu-id="0d3cf-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="0d3cf-113">Wenn Sie änderungen an den oben genannten Registrierungsschlüsseln vornehmen, um TLS 1.2 zu aktivieren, starten Sie den Server neu, damit die Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="0d3cf-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="0d3cf-114">Stellen Sie außerdem sicher, dass Die neuesten Windows- und Exchange-Updates installiert sind.</span><span class="sxs-lookup"><span data-stu-id="0d3cf-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="0d3cf-115">Weitere Informationen finden Sie hier:</span><span class="sxs-lookup"><span data-stu-id="0d3cf-115">For more information, see:</span></span>

- [<span data-ttu-id="0d3cf-116">Exchange Server TLS Guidance, Teil 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="0d3cf-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="0d3cf-117">Exchange Server TLS-Leitfaden Teil 2: Aktivieren von TLS 1.2 und Identifizieren von Clients, die es nicht verwenden – Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="0d3cf-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="0d3cf-118">Grundlegendes zu E-Mail-Szenarien, wenn TLS-Versionen nicht mit Exchange Online vereinbart werden können – Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="0d3cf-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
