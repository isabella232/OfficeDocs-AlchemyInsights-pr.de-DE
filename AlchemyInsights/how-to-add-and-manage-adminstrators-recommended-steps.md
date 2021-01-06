---
title: Hinzufügen und Verwalten von Administratoren – empfohlene Schritte
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755834"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Hinzufügen und Verwalten von Administratoren – empfohlene Schritte

Basierend auf Ihrer Problembeschreibung haben wir eine Lösung für Sie gefunden. Die meisten Kunden konnten Ihr Problem selbst lösen, nachdem Sie unsere Dokumentation befolgen.

**Bearbeiten des Abonnement Administrators oder des Co-Administrators**

- Der Konto Administrator kann beide Rollen bearbeiten, während der Abonnement Administrator nur Co-Administratoren im Azure- [Portal](https://ms.portal.azure.com/#home)ändern kann.
- [Hinzufügen oder Ändern von Administratoren für Azure-Abonnements](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Aktualisieren des Abonnement Administrators oder des Co-Administrator für interne (Airs)-Abonnements**

Der Dienstadministrator oder der Co-Administrator kann diese Aktion mit den folgenden Schritten selbst ausführen:

1. Melden Sie sich beim [Azure-Portal](https://ms.portal.azure.com/#home) an, und klicken Sie im linken Blatt auf **Kostenverwaltung + Abrechnung** .
2. Klicken Sie auf das positionselement mit Ihrem Abonnement. Dadurch wird die Übersicht für Ihr Abonnement geöffnet.
3. Klicken Sie auf dem **Abonnement** -Blade auf **Eigenschaften**. 
4. Klicken Sie auf die Schaltfläche **Dienstadministrator** .
5. Geben Sie die e-Mail-Adresse des Benutzers ein, den Sie als Dienst Administrator festlegen möchten, und klicken Sie auf **OK**.

**Hinzufügen/Ändern/Entfernen eines Co-Administrators**

1. Melden Sie sich beim [Azure-Portal](https://ms.portal.azure.com/#home) als Dienst Administrator an.
2. Öffnen Sie [Abonnements](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) , und wählen Sie ein Abonnement aus. (Co-Administratoren kann nur im Abonnement Bereich zugewiesen werden.)
3. Navigieren Sie zu **Access Control (IAM)**  >  **Classic Administrators** hinzufügen Sie  >    >  **Add Co-Administrator** , um den Bereich **Co-Admin hinzufügen** zu öffnen (wenn die Option Co-Administrator hinzufügen deaktiviert ist, bedeutet dies, dass Sie nicht über Berechtigungen verfügen).
4. Wählen Sie den Benutzer aus, den Sie hinzufügen möchten, und klicken Sie auf **Hinzufügen**.

**Weitere Informationen:**
- [Hinzufügen eines Co-Administrators](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Entfernen eines Co-Administrators](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Ändern des Dienstadministrators](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Anzeigen des Konto Administrators](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Verwalten des Zugriffs über RBAC und Azure-Portal](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Hinzufügen/Löschen von Benutzern mithilfe von Azure Active Directory (AD)**

Sie können neue Benutzer hinzufügen oder vorhandene Benutzer aus ihrer Azure-Active Directory (Azure AD)-Organisation löschen:

1. Um einen neuen Benutzer hinzuzufügen, melden Sie sich als Benutzer Administrator für die Organisation im [Azure-Portal](https://ms.portal.azure.com/#home) an.
2. Wählen Sie **Azure Active Directory** aus, wählen Sie **Benutzer** aus, und klicken Sie dann auf **neuer Benutzer**.
3. Füllen Sie auf der Seite **Benutzer** die erforderlichen Informationen aus. Klicken Sie auf **Erstellen**. Der Benutzer wird erstellt und dem Azure AD Mandanten hinzugefügt.

**Weitere Informationen**:

- [Hinzufügen eines neuen Benutzers](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Benutzer löschen](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Hinzufügen oder Aktualisieren der Profilinformationen eines Benutzers mithilfe von Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Empfohlene Dokumente**

- [Was ist die rollenbasierte Zugriffssteuerung (Role-Based Access Control, RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Grundlegendes zu den verschiedenen Rollen in Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Administratorrollenberechtigungen in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Lernprogramm: Gewähren des Zugriffs für einen Benutzer, der RBAC und das Azure-Portal verwendet](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Problembehandlung bei RBAC in Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Organisieren Ihrer Ressourcen mit Azure-Verwaltungsgruppen](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Anfordern einer Kopie von Azure Invoice per e-Mail](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Vorgehensweise hinzufügen, aktualisieren oder Entfernen einer Kreditkarte oder Debitkarte aus Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Abonnement verwalten (reactivate/Cancel/Switch)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



