---
title: Informationen Yammer Administratoren
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
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/22/2021
ms.locfileid: "50995261"
---
# <a name="about-yammer-admins"></a>Informationen Yammer Administratoren

**Netzwerkadministratoren**

Globale Administratoren werden automatisch in die Rolle "Überprüfter Administrator" in einem Yammer heraufgestuft. In den folgenden Fällen tritt diese Aktion möglicherweise nicht ordnungsgemäß auf:

- Mehrere Yammer vorhanden, und der Administrator wird bei der falschen angemeldet. [Die Netzwerkkonsolidierung](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) ist erforderlich, um zu einem Yammer zu kommen.
- Azure PIM wird verwendet. Der Benutzer wird möglicherweise nicht lange genug zum globalen Administrator heraufgestuft, damit die Heraufstufung stattfindet. Ein zukünftiges Update für Yammer kann dieses Problem beheben, es ist jedoch am besten, Benutzer manuell zum globalen Administrator zu bewerben.
- Es liegt ein Synchronisierungsproblem mit dem Yammer vor. In diesem Fall ist eine Supportanfrage für weitere Untersuchungen erforderlich.

Weitere Informationen zu Yammer Administratorrollen finden Sie unter [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).

**Gruppenadministratoren**

Gruppenadministratoren für mit Microsoft 365 verbundene Gruppen werden mit der Gruppenmitgliedschaft aus Azure AD synchronisiert. Bei großen Gruppen kann diese Synchronisierung einen längeren Zeitraum dauern.
