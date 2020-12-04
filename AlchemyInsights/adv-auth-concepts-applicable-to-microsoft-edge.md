---
title: Erweiterte Authentifizierungskonzepte, die für Microsoft Edge gelten
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571827"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Erweiterte Authentifizierungskonzepte, die für Microsoft Edge gelten

Im folgenden sind die erweiterten Authentifizierungskonzepte aufgeführt, die auf Microsoft Edge zutreffen:

**Proaktive Authentifizierung**

Wenn Sie die [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) -Richtlinie aktivieren, versucht Microsoft Edge die aktive Authentifizierung von angemeldeten Benutzern über Microsoft-Dienste. In regelmäßigen Abständen wird ein Onlinedienst verwendet, um nach einem aktualisierten Manifest zu suchen, das die Konfiguration für die proaktive Authentifizierung enthält.

Vorteile: die proaktive Authentifizierung ermöglicht die Authentifizierung für wichtige Dienste, wie beispielsweise die Registerkarte "Office New". Wenn Bing als Such Modul verwendet wird, verbessert die proaktive Authentifizierung auch die Leistung der Adressleiste und hilft bei der Generierung von Suchergebnissen, die auf die Anforderungen Ihres Unternehmens zugeschnitten sind.

**Windows Hello CredUI für die NTLM-Authentifizierung**

Wenn einmaliges Anmelden (Single Sign-on, SSO) nicht verfügbar ist, wenn eine Website versucht, sich über den NTLM-oder Negotiate-Mechanismus am Benutzer anzumelden, ermöglicht diese Funktion dem Benutzer, die Betriebssystem Anmeldeinformationen für die Website freizugeben und die Authentifizierungsanforderung mithilfe der Windows Hello cred-Benutzeroberfläche zu erfüllen. Dieser Anmelde Fluss wird nur in Windows 10 und nur für Benutzer angezeigt, die nicht SSO während einer NTLM-oder Negotiate-Herausforderung erhalten.

**Automatisches Anmelden mit gespeicherten Kennwörtern**

Benutzer, die Kennwörter in Microsoft Edge speichern, können die automatische Anmeldung bei Websites aktivieren, auf denen Sie Anmeldeinformationen gespeichert haben. Benutzer können diese Funktion in Edge://Settings/passwords aktivieren oder deaktivieren, und Sie können Sie in den [Password Manager-](https://go.microsoft.com/fwlink/?linkid=2134622) Richtlinien konfigurieren.
