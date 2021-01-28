---
title: Zugriffsüberprüfungen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7767"
ms.openlocfilehash: b2ba50c4f8e667f81b638ba480fa846e149c3d43
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013948"
---
# <a name="access-reviews"></a>Zugriffsüberprüfungen

1. **Aktivieren von Zugriffsüberprüfungen:** Sie können Rezensionen aktivieren, wenn Sie ein neues Zugriffspaket erstellen oder ein vorhandenes Zugriffspaket bearbeiten. [Erstellen einer Zugriffsüberprüfung eines Zugriffspakets in Azure AD-Berechtigungsverwaltung](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) beschreibt, wie Zugriffsüberprüfungen von Zugriffspaketen aktiviert werden.

1. **Zugriff überprüfen:** Azure AD-Berechtigungsverwaltung vereinfacht die Verwaltung des Zugriffs auf Gruppen, Anwendungen und SharePoint-Websites. [Das Überprüfen des Zugriffs](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) auf ein Zugriffspaket in der Azure AD-Berechtigungsverwaltung beschreibt, wie Zugriffsüberprüfungen für andere Benutzer ausgeführt werden, die einem Zugriffspaket als festgelegter Prüfer zugewiesen sind.

1. **Review Access for Yourself**: [Self-review of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-self-review) describes how a user does a self-review of their assigned access package(s).

1. In den meisten Fällen finden Endbenutzer eine Rezension, die ihre Antwort in **der Zugriffsteuerung aussteht.** Dies gilt nur für Rezensionen von Gruppen und Anwendungen, nicht für Rollen. Für alle Zugriffsüberprüfungen von Rollen müssen Endbenutzer zu Azure AD Privileged Identity Management (PIM) navigieren, um ihre Überprüfung abschließen zu können.

    1. Anmelden beim Azure-Portal.
    2. Navigieren Sie zu Azure AD PIM.
    3. Wählen Sie im linken Navigationsbereich den Zugriff **"Aufgaben**  >  **überprüfen" aus.**
    
Weitere Informationen finden Sie unter:

- [Durchführen einer Zugriffsüberprüfung meiner Azure AD-Verzeichnisrollen in PIM ](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-perform-security-review/)
- [Durchführen einer Zugriffsüberprüfung meiner Azure-Ressourcenrollen in PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-perform-access-review/)