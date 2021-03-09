---
title: Problem beim Zurücksetzen des Kennworts
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: fe3a13acb0ba5c8872d7c0bb8c3961d83f7d3526
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568582"
---
# <a name="problems-resetting-password"></a>Probleme beim Zurücksetzen des Kennworts

Nachfolgend finden Sie einige der Probleme, die beim Zurücksetzen des Kennworts auftreten können, und die möglichen Lösungen:

**Ich habe ein Problem mit der Kennwortzurücksetzung, das in den anderen Kategorien nicht behandelt wird**

-Stellen Sie sicher, dass Sie autorisiert sind, Kennwörter zurückzusetzen. Nur globale, Kennwort- und Benutzeradministratoren können Benutzerkennwörter zurücksetzen. Globale Administratoren können auch die Kennwörter anderer privilegierter Administratoren zurücksetzen.
- Stellen Sie sicher, dass Sie die Lizenzierungsanforderungen verstehen:
    - In Ihrer Organisation muss mindestens eine Lizenz zugewiesen sein.
        - Nur Cloudbenutzer – Office 365 (O365) kostenpflichtige SKU oder Azure AD Basic
        - Cloud- und/oder lokale Benutzer – Azure AD Premium P1 oder P2, Enterprise Mobility + Security (EMS) oder Secure Productive Enterprise (SPE)
        - Weitere Informationen zu Lizenzierungsanforderungen finden Sie im Artikel [Lizenzierungsanforderungen für die Self-Service-Kennwortzurücksetzung von Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ich habe Probleme beim Testen der von mir festgelegten Kennwortzurücksetzungsrichtlinie**

- Kürzlich angewendete Richtlinien können mehrere Minuten dauern, bis sie über alle Rechenzentren und Endpunkte repliziert werden. Der physische Abstand zum Rechenzentrum wirkt sich auch darauf aus, wie schnell Änderungen angewendet werden.
- Testen Sie mit einem Endbenutzer, nicht mit einem Administrator, und testen Sie mit einer kleinen Gruppe von Benutzern. Die im Azure-Portal konfigurierten Richtlinien gelten nur für Endbenutzer, nicht für Administratoren. Microsoft erzwingt eine starke standardmäßige Zwei-Tore-Kennwortzurücksetzungsrichtlinie für alle Azure-Administratorrolle (Beispiel: Globaler Administrator, Helpdeskadministrator, Kennwortadministrator usw.)
    - Erfahren Sie mehr über [Richtlinien für Administratoren](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).

**Ich möchte die Kennwortzurücksetzung bereitstellen, möchte aber nicht, dass meine Benutzer zusätzliche Sicherheitsinformationen registrieren.**

Füllen Sie Daten für Ihre Benutzer vorab auf, damit sie dies nicht müssen! – Als Administrator können Sie Telefon- und E-Mail-Eigenschaften für Ihre Benutzer festlegen, bevor Sie die Kennwortzurücksetzung für Ihre Organisation durchführen. Sie können dies mithilfe einer API, PowerShell oder Azure AD Connect tun. Weitere Informationen finden Sie hier:
- [Bereitstellen der Kennwortzurücksetzung, ohne dass Benutzer sich registrieren müssen](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Welche Daten bei der Kennwortzurücksetzung verwendet werden](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Die Schaltfläche zum Zurücksetzen des Kennworts ist ausgegraut.**

Sie sind nicht autorisiert, die Kennwörter dieses Benutzers zurückzusetzen. Nur globale, Kennwort- und Benutzeradministratoren können Benutzerkennwörter zurücksetzen. Globale Administratoren können auch die Kennwörter anderer privilegierter Administratoren zurücksetzen.

**Das Blatt zum Zurücksetzen des Kennworts wird nicht angezeigt.**

Sie sind nicht autorisiert, Kennwörter zurückzusetzen. Nur globale, Kennwort- und Benutzeradministratoren können Benutzerkennwörter zurücksetzen. Globale Administratoren können auch die Kennwörter anderer privilegierter Administratoren zurücksetzen.

**Das lokale Integrationsblatt wird bei der Kennwortzurücksetzung nicht angezeigt.**

- Das lokale Integrationsblatt wird nur in Hybridumgebungen angezeigt, d. h. Sie verwenden das Kennwortrückschreiben, um die Kennwörter des lokalen Benutzers zu bearbeiten.
- Dieses Blatt wird nicht angezeigt, wenn:
    - Kennwortrückschreiben wird nicht verwendet
    - Es liegt ein Problem mit der Installation/Konnektivität des Kennwortrückschreibens vor.
    - Es liegt ein Problem mit der Installation/Konnektivität von Azure AD Connect vor.
    - Weitere Schritte zur Problembehandlung bei Problemen mit dem Kennwortrückschreiben finden Sie im Abschnitt Problembehandlung beim [Kennwortrückschreiben.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ich weiß nicht, wie das Kennwort eines Benutzers zurückgesetzt wird**

1. Melden Sie sich beim Azure-Portal als geeigneter Administrator an.
1. Wechseln Sie zum Blatt Benutzer und Gruppen, wählen Sie **Alle Benutzer aus.**
1. Wählen Sie einen Benutzer aus der Liste aus.
1. Wählen Sie für den ausgewählten Benutzer **Übersicht** aus, und klicken Sie dann in der Befehlsleiste auf **Kennwort zurücksetzen.**
1. Folgen Sie den Anweisungen auf dem Bildschirm.
    - Nur über das Azure-Portal durchgeführte Zurücksetzen unterstützen das Kennwortrückschreiben.

**Ich habe das Kennwort eines lokalen Benutzers über das Office 365 Admin-Portal oder die mobile Office 365-Anwendung zurückgesetzt, aber der Benutzer kann sich weiterhin nicht anmelden.**

Kennwortrückschreiben wird in diesem Portal nicht unterstützt. Setzen Sie das Kennwort des Benutzers im Azure-Portal erneut zurück – portal.azure.com

