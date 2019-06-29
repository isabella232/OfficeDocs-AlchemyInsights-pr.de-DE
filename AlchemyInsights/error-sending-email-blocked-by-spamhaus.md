---
title: Fehler beim Senden von e-Mails, die von Spamhaus blockiert wurden
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 52a5c20d59a2eac4c4bf465edaa888952d47f39f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35387848"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Fehler beim Senden von e-Mail: Client Host blockiert mit Spamhaus

Die IP-Adresse, die die Nachricht gesendet hat, befindet sich in einer Sperrliste im Besitz von [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Gründe für die Blockierung durch Spamhaus sind kompromittierte Konten, gefährdete Computer, die eine öffentliche IP-Adresse teilen, und Richtlinien für Internetdienstanbieter (ISP). Mögliche Korrekturen sind:
  
- Für blockierte eingehende Nachrichten an Office 365, in dem Sie den Quell-e-Mail-Server steuern, müssen Sie die Ursache ermitteln und den Block von der Spamhaus-Website entfernen.

- Für blockierte eingehende Nachrichten an Office 365, bei denen die Quell-IP-Adresse einer anderen Person gehört, muss der Adress Besitzer den Block von der Spamhaus-Website entfernen. Wenn sich die IP-Adresse in der Richtlinien Sperrliste befindet (PBL), kann der Besitzer eine andere statische IP-Adresse zuweisen oder die Adresse aus dem PBL entfernen.

- Bei blockierten ausgehenden Nachrichten von Ihrer Office 365 Domäne können Sie diesen Fehler erhalten, wenn die Nachrichten über einen Drittanbieterdienst weitergeleitet werden. Sie können ein Whois-Nachschlage Tool verwenden, um den Besitzer blockierter IP-Adressen zu finden.
