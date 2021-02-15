---
title: Gruppenrichtlinie
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2021
ms.locfileid: "50243903"
---
# <a name="group-policy"></a>Gruppenrichtlinie

Einstellungen für Benutzer- und Computerobjekte in Azure Active Directory Domain Services (Azure AD DS) werden häufig mit Gruppenrichtlinienobjekten (GPOs) verwaltet. Azure AD DS enthält integrierte GPOs für die Container "AADDC-Benutzer" und "AADDC-Computer". Sie können diese integrierten Gruppenrichtlinienobjekte anpassen, um Gruppenrichtlinien nach Bedarf für Ihre Umgebung zu konfigurieren. Mitglieder der Gruppe der Azure AD DC-Administratoren verfügen in der Azure AD DS-Domäne über Administratorrechte für Gruppenrichtlinien und können auch benutzerdefinierte Gruppenrichtlinienobjekte und Organisationseinheiten erstellen. Weitere Informationen darüber, was eine Gruppenrichtlinie ist und wie sie funktioniert, finden Sie unter [Gruppenrichtlinienübersicht](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

In einer Hybridumgebung werden in einer lokalen AD DS-Umgebung konfigurierte Gruppenrichtlinien nicht mit Azure AD DS synchronisiert. Um Konfigurationseinstellungen für Benutzer oder Computer in Azure AD DS zu definieren, bearbeiten Sie eines der Standardrichtlinienobjekte, oder erstellen Sie ein benutzerdefiniertes Gruppenrichtlinienobjekt.

In diesem Artikel, [Verwalten von Gruppenrichtlinienrichtlinien](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) wird gezeigt, wie Sie die Tools für die Gruppenrichtlinienverwaltung installieren, die integrierten Gruppenrichtlinienobjekte bearbeiten und wie benutzerdefinierte Gruppenrichtlinienobjekte erstellt werden.



