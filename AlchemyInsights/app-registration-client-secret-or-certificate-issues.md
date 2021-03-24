---
title: Geheime Client- oder Zertifikatprobleme bei der App-Registrierung
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123116"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Geheime Client- oder Zertifikatprobleme bei der App-Registrierung

Ablauf des Geheimen Anwendungsclients?

Unabhängig davon, wie die registrierte Anwendung erstellt wurde, sei es über den Standardregistrierungsprozess im Apps-Registrierungsportal oder wenn der Dienstprinzipal in Ihrem Mandanten mithilfe der Anwendungs zustimmung erstellt wurde, muss ein neuer Geheimer Clientgeheimnis vor dem Ablauf des aktuellen erstellt und im zugehörigen Anwendungscode aktualisiert werden. Die maximale Gültigkeitsdauer beträgt 2 Jahre. Zur Erinnerung: Der geheime Wert muss aufgezeichnet werden, da er nach dem Verlassen der Seite "App-Registrierungen" im Portal nicht mehr sichtbar ist. Weitere Informationen finden Sie unter [Schnellstart: Registrieren einer App in](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) der Microsoft Identity Platform und Bewährte Methoden für die Microsoft Identity [Platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).

Weitere Informationen finden Sie unter [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).
