---
title: Fehler beim Senden von von SpamHaus blockierten E-Mails
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813723"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Fehler beim Senden von E-Mails: Clienthost mit Spamhaus blockiert

Die IP-Adresse, die die Nachricht gesendet hat, befindet sich in einer Sperrliste im Besitz von [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Gründe für das Blockieren durch Spamhaus sind gefährdete Konten, gefährdete Computer, die eine öffentliche IP-Adresse freigeben, und Internetdienstanbieterrichtlinien. Mögliche Korrekturen sind:
  
- Bei blockierten eingehenden Nachrichten, auf denen Sie den Quell-E-Mail-Server steuern, müssen Sie die Ursache ermitteln und den Block von der Spamhaus-Website entfernen.

- Bei blockierten eingehenden Nachrichten, bei denen die Quell-IP-Adresse zu einer anderen Person gehört, muss der Adressbesitzer den Block von der Spamhaus-Website entfernen. Wenn sich die IP-Adresse in der Richtlinienblockierungsliste (Policy Block List, PBL) befindet, kann der Besitzer eine andere statische IP-Adresse zuweisen oder die Adresse aus der PBL entfernen.

- Bei blockierten ausgehenden Nachrichten aus Ihrer mit Microsoft verbundenen Domäne können Sie diesen Fehler erhalten, wenn die Nachrichten über einen Drittanbieterdienst geroutet werden. Sie können ein WHOIS-Suchtool verwenden, um den Besitzer der blockierten IP-Adresse zu finden.
