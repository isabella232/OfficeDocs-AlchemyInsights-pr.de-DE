---
title: Automatische Anmeldung bei Microsoft Edge
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
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398728"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automatische Anmeldung bei Microsoft Edge

Microsoft Edge verwendet das Standardkonto des Betriebssystems, um sich automatisch bei einem Benutzer entsprechend der Konfiguration des Geräts des Benutzers zu anmelden. 

Die Szenarien der einzelnen Gerätekonfigurationen und des abhängigen Benutzer-Anmeldevorgangs werden unten beschrieben:

- **Das Gerät ist hybrid/AAD-J**: Diese Option ist unter Windows 10, windows-down-level und entsprechenden Serverversionen verfügbar. Benutzer werden automatisch mit ihren Azure Active Directory (AD)-Konten angemeldet.
- **Das Gerät ist mit der Domäne** verbunden: Diese Option ist unter Windows 10, Windows auf down-Level-Ebene und entsprechenden Serverversionen verfügbar. Standardmäßig werden Benutzer mit Domänenkonten nicht automatisch angemeldet. Verwenden Sie die **ConfigureOnPremisesAccountAutoSignIn-Richtlinie,** um die automatische Anmeldung für sie zu aktivieren. Um die automatische Anmeldung für Benutzer mit Azure AD-Konten zu aktivieren, sollten Sie die Hybridinteging ihrer Geräte in Betracht ziehen.
- Das **Standardkonto** des Betriebssystems ist ein Microsoft-Konto: Diese Option ist unter Windows 10 RS3 (Version 1709, Build 10.0.16299) und höher verfügbar. Das Szenario wird auf Unternehmensgeräten wahrscheinlich nicht auftreten. Wenn es sich bei dem Standardkonto des Betriebssystems jedoch um ein Microsoft-Konto handelt, wird microsoft Edge den Benutzer automatisch mit dem Microsoft-Konto anmelden.
 
 
