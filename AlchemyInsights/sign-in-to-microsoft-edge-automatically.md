---
title: Automatisches Anmelden bei Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599468"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automatisches Anmelden bei Microsoft Edge

Microsoft Edge verwendet das Standardkonto des Betriebssystems, um sich automatisch bei einem Benutzer anzumelden, je nachdem, wie das Gerät des Benutzers konfiguriert ist. 

Die Szenarien der einzelnen Geräte Konfigurationstypen und des abhängigen Benutzeranmeldeprozesses werden im folgenden beschrieben:

1. **Das Gerät ist Hybrid/Aad-J**: diese Option ist unter Windows 10, untergeordnete Fenster und entsprechende Server Versionen verfügbar. Benutzer werden automatisch mit ihren Azure-Active Directory Konten (AD) angemeldet.
2. **Das Gerät ist Domänenbeitritt**: diese Option ist unter Windows 10, untergeordnete Fenster und entsprechende Server Versionen verfügbar. Standardmäßig werden Benutzer mit Domänenkonten nicht automatisch angemeldet; um die automatische Anmeldung für diese zu aktivieren, verwenden Sie die **ConfigureOnPremisesAccountAutoSignIn** -Richtlinie. Wenn Sie die automatische Anmeldung für Benutzer mit Azure Ad Konten aktivieren möchten, sollten Sie den Hybriden Beitritt zu Ihren Geräten in Frage stellen.
3. **Das Standardkonto des Betriebssystems ist ein Microsoft-Konto**: diese Option ist unter Windows 10 RS3 (Version 1709, Build 10.0.16299) und höheren Versionen verfügbar. Das Szenario ist unwahrscheinlich, dass es auf Enterprise-Geräten auftritt. Wenn das Standardkonto des Betriebssystems jedoch ein Microsoft-Konto ist, meldet sich Microsoft Edge automatisch beim Benutzer mit dem Microsoft-Konto an.
 
 
