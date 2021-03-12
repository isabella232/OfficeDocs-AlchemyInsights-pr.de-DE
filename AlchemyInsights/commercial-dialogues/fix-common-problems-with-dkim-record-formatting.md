---
title: Beheben häufiger Probleme bei der Formatierung von DKIM-Eintragen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737177"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Beheben häufiger Probleme bei der Formatierung von DKIM-Eintragen

Die meisten DkIM-Einrichtungsprobleme stehen im Zusammenhang mit falschen DNS-Einträgen.

Um die #A0 zu beheben, stellen Sie sicher, dass der DKIM-CNAME-Eintrag **(kein** #A1) richtig formatiert ist. Weitere Informationen finden Sie unter Was Sie zum manuellen Einrichten von [DKIM in Office 365 tun müssen.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Wenn Sie Hilfe bei DNS-Einträgen im Allgemeinen benötigen, lesen Sie Erstellen von [DNS-Einträgen bei einem beliebigen DNS-Hostinganbieter für Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

> [!NOTE]
> Nachdem Sie Ihre DKIM-DNS-Einträge beim DNS-Hostingdienst für Ihre Domäne erstellt oder aktualisiert haben, müssen Sie warten, bis die DNS-Einträge veröffentlicht werden.
