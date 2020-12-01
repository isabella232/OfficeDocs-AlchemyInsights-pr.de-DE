---
title: Mandant löschen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/30/2020
ms.locfileid: "49477676"
---
# <a name="delete-tenant"></a>Mandant löschen

Um eine Azure AD zu löschen, stellen Sie Folgendes sicher:
- Sie sind ein globaler Administrator für das Verzeichnis.
- Sie sind nicht mit einem Konto angemeldet, das über das Standardverzeichnis wie contoso.onmicrosoft.com im angemeldeten Konto verfügt, beispielsweise admin@contoso.onmicrosoft.com.
- Entfernen Sie alle aktiven Anwendungen in dem Verzeichnis vor dem Löschen. Wenn Sie aktive Anwendungen entfernen möchten, navigieren Sie zu app-Registrierungen, und entfernen Sie die vorhandenen Anwendungen.
- Es sind keine aktiven Abonnements für Microsoft Online Services vorhanden, wie Microsoft Azure, Office 365 oder Azure AD Premium, die dem Verzeichnis zugeordnet sind. Übertragen Sie Ihre Abonnements oder beschleunigen Sie die Löschung aktiver Abonnements über Azure-Unterstützung und Abrechnung. Erfahren Sie mehr über das Abbrechen von Office 365-und Azure-Abonnements. Anleitungen zum Zuordnen oder Hinzufügen eines vorhandenen Abonnements zu einem Mandanten finden Sie unter [Associate or Add a Azure Subscription to your Azure AD Mandanten](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Es gibt keine aktive Lizenz. Informationen zum Entfernen von Lizenzen finden Sie unter [Entfernen eines Abonnements zum Entfernen der Lizenz](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Es gibt keine anderen aktiven Benutzer im Verzeichnis als den globalen Administrator, wenn Sie versuchen, die Azure AD zu löschen. Entfernen Sie alle anderen aktiven Benutzer, und alle Abhängigkeiten von einem benutzerdefinierten Domänennamen im Mandanten müssen ebenfalls entfernt werden, beispielsweise Benutzer, die mit admin@contoso.com erstellt werden.

Ausführlichere Informationen zu den folgenden Schritten:
- Delete "Azure Active Directory" oder "Subscription" finden Sie unter [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Entfernen von Anwendungen im Verzeichnis finden Sie unter [Entfernen von Anwendungen](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
