---
title: Problem mit Sicherheitsgruppen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162926"
---
# <a name="issue-with-security-groups"></a>Problem mit Sicherheitsgruppen

**Wenn Sie Netzwerkfehler des Typs AADDS104 erhalten**

Ungültige Regeln für Netzwerksicherheitsgruppen sind die häufigste Ursache für Netzwerkfehler in Azure Active Directory Domain Services (AD DS). Die Netzwerksicherheitsgruppe für das virtuelle Netzwerk muss den Zugriff auf bestimmte Ports und Protokolle zulassen. Wenn diese Ports blockiert sind, kann die Azure-Plattform die verwaltete Domäne nicht überwachen oder aktualisieren. Die Synchronisierung zwischen Azure AD und Azure AD DS ist ebenfalls betroffen. Stellen Sie sicher, dass die Standardports geöffnet bleiben, um Dienstunterbrechungen zu vermeiden.

Informationen zum Verstehen und Beheben häufiger Warnungen zu Konfigurationsproblemen bei der Netzwerksicherheitsgruppe finden Sie unter [Hinzufügen und Überprüfen von Sicherheitsgruppen](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).
