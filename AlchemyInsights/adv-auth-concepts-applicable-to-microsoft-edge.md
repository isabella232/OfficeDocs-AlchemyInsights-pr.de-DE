---
title: Erweiterte Authentifizierungskonzepte für Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398560"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Erweiterte Authentifizierungskonzepte für Microsoft Edge

Nachfolgend finden Sie die erweiterten Authentifizierungskonzepte, die für Microsoft Edge gelten:

**Proaktive Authentifizierung**

Wenn Sie die [ProaktiveAuthEnabled-Richtlinie](https://go.microsoft.com/fwlink/?linkid=2134621) aktivieren, versucht Microsoft Edge, angemeldete Benutzer proaktiv über Microsoft-Dienste zu authentifizieren. In regelmäßigen Abständen wird ein Onlinedienst verwendet, um nach einem aktualisierten Manifest zu suchen, das die Konfiguration für die proaktive Authentifizierung enthält.

Vorteile: Die proaktive Authentifizierung ermöglicht die Authentifizierung für wichtige Dienste, z. B. die Office New Tab Page. Wenn Bing als Suchmaschine verwendet wird, verbessert die proaktive Authentifizierung außerdem die Leistung der Adressleiste und hilft bei der Generierung von Suchergebnissen, die auf die Anforderungen Ihres Unternehmens zugeschnitten sind.

**Windows Hello CredUI für die NTLM-Authentifizierung**

Wenn einmaliges Anmelden (Single Sign-On, SSO) nicht verfügbar ist, wenn eine Website versucht, sich über den NTLM- oder Negotiate-Mechanismus beim Benutzer zu registrieren, ermöglicht dieses Feature dem Benutzer, die Anmeldeinformationen des Betriebssystems für die Website frei zu geben und die Authentifizierungsanforderungen mithilfe der Windows Hello Cred-Benutzeroberfläche zu erfüllen. Dieser Anmeldefluss wird nur unter Windows 10 und nur für Benutzer angezeigt, die während eines NTLM oder einer Negotiate-Herausforderung keine SSO erhalten.

**Automatische Anmeldung mit gespeicherten Kennwörtern**

Benutzer, die Kennwörter in Microsoft Edge speichern, können die automatische Anmeldung bei Websites aktivieren, auf denen sie Anmeldeinformationen gespeichert haben. Benutzer können dieses Feature in edge://settings/passwords aktivieren oder deaktivieren, und Sie können es in den [Kennwort-Manager-Richtlinien](https://go.microsoft.com/fwlink/?linkid=2134622) konfigurieren.
