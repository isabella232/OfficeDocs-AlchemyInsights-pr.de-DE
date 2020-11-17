---
title: Rolle "privilegierte Identitätsverwaltung"
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086376"
---
# <a name="privileged-identity-managementpim-role"></a>Rolle "PIM (Privileged Identity Management)"

**Berechtigungen werden nach dem Aktivieren einer Rolle nicht erteilt.**

Wenn Sie eine Rolle in Azure AD privilegierten Identitätsverwaltung (PIM) aktivieren, wird die Aktivierung möglicherweise nicht sofort an alle Portale weitergegeben, die die privilegierte Rolle benötigen. In einigen Fällen kann es vorkommen, dass die Änderung nicht sofort wirksam wird, auch wenn die Änderung weitergegeben wird.

Wenn Ihre Aktivierung verzögert wird, führen Sie die folgenden Schritte aus:

1. Melden Sie sich im Azure-Portal ab, und melden Sie sich dann wieder an. Wenn Sie eine Azure AD Rolle oder eine Azure-Ressourcenrolle aktivieren, werden die Phasen der Aktivierung angezeigt. Sobald alle Phasen abgeschlossen sind, wird der Link "Abmelden" angezeigt. Sie können diesen Link verwenden, um sich abzumelden. Dadurch werden die meisten Fälle für die Aktivierungsverzögerung gelöst.
2. Stellen Sie in PIM sicher, dass Sie als Mitglied der Rolle aufgeführt sind.
3. Wenn Sie die Rolle Exchange-Administrator aktivieren, stellen Sie sicher, dass Sie sich abmelden und wieder anmelden. Wenn das Problem weiter besteht, öffnen Sie ein Support Ticket, und stellen Sie dieses als Problem herauf. Wenn Sie Ihre Exchange-Administrator Rolle für den Zugriff auf das Security and Compliance Center verwenden, lesen Sie den nächsten Schritt.
4. Wenn Sie eine Rolle für den Zugriff auf das Security and Compliance Center aktivieren oder die SharePoint-Administrator Rolle aktivieren, tritt eine Aktivierungsverzögerung von ein paar Minuten bis zu einigen Stunden ein. Dies ist ein bekanntes Problem, und wir arbeiten aktiv mit diesen Teams zusammen, um dieses Problem so schnell wie möglich zu beheben.

Weitere Informationen finden Sie unter:

- [Aktivieren von "meine Azure AD"-Rollen in PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Aktivieren von My Azure Resource Roles in PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Berechtigungen werden nach dem Deaktivieren einer Rolle nicht entfernt, oder die Rollen Aktivierung läuft ab.**

Wenn Sie eine Rolle in Azure AD privilegierten Identitätsverwaltung oder beim Ablauf einer Rollen Aktivierungs Periode deaktivieren, kann es zu Verzögerungen kommen, in denen Sie weiterhin auf Zugriff haben.

Wenn Ihre Deaktivierung verzögert wird, führen Sie die folgenden Schritte aus:

1. Wenn Sie die Exchange-Administrator Rolle deaktivieren oder der Aktivierungszeitraum für die Rolle abgelaufen ist und Sie eine erhebliche Verzögerung feststellen, bevor die Berechtigungen entfernt wurden, öffnen Sie ein Support Ticket, und teilen Sie Ihrem Supporttechniker mit, wie Sie ein Ticket mit dem Team für die privilegierte Zugriffsverwaltung ("PAM") in Office zu diesem Problem einreichen können.
2. Wenn der Aktivierungszeitraum abgelaufen ist, Sie aber dennoch die Browsersitzung geöffnet haben, schließen Sie den Browser. Sie können die Rolle weiterhin verwenden, bis Sie diese Sitzung schließen. Dies ist ein bekanntes Problem, und wir suchen eine mögliche Lösung, um jede Sitzung aktiv aufzuheben, nachdem die Aktivierung abgelaufen ist.

Wenn sich Ihre Verzögerung von diesen beiden Szenarien unterscheidet, öffnen Sie ein Support Ticket.
