---
title: Abonnement Zugriff
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/27/2020
ms.locfileid: "48773774"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Das Anmelden in Azure kann aufgrund von Browserproblemen nicht möglich sein (Browser hängt, dreht sich weiter, wird nicht herunterladen usw.)

Möglicherweise sind Sie von einem Ausfall betroffen. Überprüfen Sie, ob ein ständiger Ausfall vorliegt: [Azure-Integritäts Status](https://status.azure.com/status/history/).

Melden Sie sich bei allen aktiven Azure-Sitzungen ab. Starten Sie einen in-private-oder Inkognito-Modus Ihres Webbrowsers.

Sie können auch versuchen, Browser zu aktualisieren, einen anderen Browser zu verwenden, Cache-Cookies zu löschen, wenn oben nicht funktioniert.

Weitere Informationen: [Problembehandlung bei Anmeldeproblemen](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Zugriff auf Abonnements nicht möglich**

Stellen Sie im [Azure-Portal](https://portal.azure.com/)sicher, dass das richtige Azure-Verzeichnis aus dem Konto oben rechts ausgewählt ist.

Stellen Sie im [Azure-Konto Center](https://account.windowsazure.com/Subscriptions)sicher, dass das verwendete Konto der Konto Administrator ist.

Weitere Informationen: [Problembehandlung bei nicht gefundenen Abonnements](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Zugriff auf Abrechnungsverlauf nicht möglich**

Der Konto Administrator muss sicherstellen, dass der Benutzer, der auf die Abrechnungsinformationen zugreift, im Azure Active Directory als Gastbenutzer hinzugefügt wird: [einen neuen Benutzer hinzufügen oder löschen](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Dem Benutzer muss dann eine globale Administratorrolle zugewiesen werden: [Zuweisen von Rollen zu Benutzern](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Veröffentlichen Sie dies, kann dem Benutzer mithilfe von RBAC-Richtlinien ein Abrechnungs Zugriff gewährt werden: [gewähren des Zugriffs auf die Abrechnung](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Empfohlene Dokumente**

-   [Ich kann mich nicht zum Verwalten des Azure-Abonnements anmelden.](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)