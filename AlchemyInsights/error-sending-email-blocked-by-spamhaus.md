---
title: Fehler beim Senden von e-Mails, die von Spamhaus blockiert wurden
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714257"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Fehler beim Senden von e-Mail: Client Host blockiert mit Spamhaus

Die IP-Adresse, die die Nachricht gesendet hat, befindet sich in einer Sperrliste im Besitz von [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Gründe für die Blockierung durch Spamhaus sind kompromittierte Konten, gefährdete Computer, die eine öffentliche IP-Adresse teilen, und Richtlinien für Internetdienstanbieter (ISP). Mögliche Korrekturen sind:
  
- Bei blockierten eingehenden Nachrichten, bei denen Sie den Quell-e-Mail-Server steuern, müssen Sie die Ursache ermitteln und den Block von der Spamhaus-Website entfernen.

- Bei blockierten eingehenden Nachrichten, bei denen die Quell-IP-Adresse einer anderen Person gehört, muss der Adress Besitzer den Block von der Spamhaus-Website entfernen. Wenn sich die IP-Adresse in der Richtlinien Sperrliste befindet (PBL), kann der Besitzer eine andere statische IP-Adresse zuweisen oder die Adresse aus dem PBL entfernen.

- Bei blockierten ausgehenden Nachrichten von ihrer mit Microsoft verbundenen Domäne können Sie diesen Fehler erhalten, wenn die Nachrichten über einen Drittanbieterdienst weitergeleitet werden. Sie können ein Whois-Nachschlage Tool verwenden, um den Besitzer blockierter IP-Adressen zu finden.
