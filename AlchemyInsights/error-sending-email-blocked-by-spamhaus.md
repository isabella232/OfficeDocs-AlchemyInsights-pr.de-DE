---
title: Fehler beim Senden von e-Mails, die von SpamHaus blockiert wurden
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 7d6ad2667613ae948a4abcefafe8d91cf89d2418
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402258"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Fehler beim Senden von e-Mails: Client Host mit Spamhaus blockiert

Die IP-Adresse, die die Nachricht gesendet hat, befindet sich in einer Sperrliste von [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Gründe für die Blockierung durch Spamhaus sind kompromittierte Konten, kompromittierte Computer mit einer öffentlichen IP-Adresse und InternetdienstAnbieter-Richtlinien. Mögliche Korrekturen sind:
  
- Für blockierte eingehende Nachrichten an Office 365, bei denen Sie den Quell-e-Mail-Server steuern, müssen Sie die Ursache ermitteln und den Block aus der Spamhaus-Website entfernen.
    
- Für blockierte eingehende Nachrichten an Office 365, bei denen die Quell-IP-Adresse zu einer anderen Person gehört, muss der Adress Besitzer den Block von der Spamhaus-Website entfernen. Wenn sich die IP-Adresse in der Richtlinien Sperrliste (PBL) befindet, kann der Besitzer eine andere statische IP-Adresse zuweisen oder die Adresse aus dem PBL entfernen.
    
- Für blockierte ausgehende Nachrichten von Ihrer Office 365-Domäne können Sie diese Fehlermeldung erhalten, wenn die Nachrichten über einen Drittanbieterdienst weitergeleitet werden. Sie können ein WHOIS-Nachschlage Tool verwenden, um den blockierten IP-Adress Besitzer zu finden.
    

