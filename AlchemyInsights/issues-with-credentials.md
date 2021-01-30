---
title: Probleme mit Anmeldeinformationen
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052948"
---
# <a name="issues-with-credentials"></a>Probleme mit Anmeldeinformationen

Microsoft Identity Platform und der [OAuth 2.0-Clientanmeldeinformationsfluss](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) beschreiben, wie Sie direkt mit dem OAuth 2.0-Client-Anmeldeinformations-Genehmigungsfluss programmieren.

**Wie verwalte ich das Kennwort oder die Zertifikatanmeldeinformationen einer Anwendung?**

In der Azure CLI können Sie az [ad-App-Anmeldeinformationen](https://docs.microsoft.com/cli/azure/ad/app/credential) verwenden, um das Kennwort oder das Zertifikat einer Anwendung zu löschen, auflisten oder zurückzusetzen.

**Wie setzen meine Benutzer ihre Kennwörter zurück?**

Benutzer müssen sich [für die Self-Service-Kennwortzurücksetzung registrieren,](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) bevor sie ihre Kennwörter zurücksetzen können. Nachdem sich ein Benutzer registriert hat, kann er den Anweisungen in diesem Artikel folgen, um sein Kennwort zurückzusetzen: [Zurücksetzen des Arbeits-](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)oder Schulkennworts.

**Wie ändern meine Benutzer ihre Kennwörter?**

Benutzer können die Schritte in diesem Artikel ausführen, um ihre Kennwörter zu ändern: [So ändern Sie Ihr Kennwort.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
Sie können auch [App-Kennwörter für die Überprüfung in zwei Schritten verwalten.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Mein Benutzer wird beim Ändern oder Zurücksetzen des Kennworts einen Fehler erhalten.**

Dieser Link enthält Informationen zu häufigen Problemen, die auftreten können, wenn ein Benutzer versucht, sein Kennwort zurückzusetzen: Häufige [Probleme und deren Lösungen](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Ich habe ein Problem beim Zurücksetzen des Kennworts eines Benutzers**

- Stellen Sie sicher, dass Sie zum Zurücksetzen von Kennwörtern autorisiert sind. *Nur globale, Kennwort- und Benutzeradministratoren können Benutzerkennwörter zurücksetzen.* Globale Administratoren können auch die Kennwörter anderer privilegierter Administratoren zurücksetzen.

- Stellen Sie sicher, dass Sie die Lizenzierungsanforderungen verstehen:

  - Ihnen muss mindestens eine Lizenz in Ihrer Organisation zugewiesen sein:
    - **Nur Cloudbenutzer** – jede kostenpflichtige Office 365 (O365)-SKU oder Azure AD Basic
    - **Cloud- und/oder lokale** Benutzer – Azure AD Premium P1 oder P2, Enterprise Mobility + Security (EMS) oder Secure Productive Enterprise (SPE)
    - Weitere Informationen zu Den Lizenzierungsanforderungen finden Sie unter Lizenzierungsanforderungen für die [Self-Service-Kennwortzurücksetzung in Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Um das Kennwort eines Benutzers zurückzusetzen, suchen Sie den Benutzer in Azure AD. Klicken Sie dann auf dem Blatt "Übersicht" für diesen Benutzer auf die Schaltfläche "Kennwort zurücksetzen".

**Die Schaltfläche zum Zurücksetzen des Kennworts ist ausgegraut.**

Sie sind nicht autorisiert, die **Kennwörter dieses** Benutzers zurückzusetzen. *Nur globale, Kennwort- und Benutzeradministratoren können Benutzerkennwörter zurücksetzen.* Globale Administratoren können auch die Kennwörter anderer privilegierter Administratoren zurücksetzen.

**Ich kann das Blatt zum Zurücksetzen des Kennworts nicht sehen.**

Sie sind nicht autorisiert, Kennwörter zurückzusetzen. *Nur globale, Kennwort- und Benutzeradministratoren können Benutzerkennwörter zurücksetzen.* Globale Administratoren können auch die Kennwörter anderer privilegierter Administratoren zurücksetzen.

**Ich kann das blatt für die lokale Integration bei der Kennwortzurücksetzung nicht sehen.**

- Das blatt für die lokale Integration wird nur in Hybridumgebungen angezeigt, d. h., Sie verwenden das Kennwortrückschreiben, um die Kennwörter der lokalen Benutzer zu bearbeiten.

- Dieses Blatt wird nicht angezeigt, wenn:

  - Sie verwenden kein Kennwortrückschreiben
  - Es liegt ein Problem mit der Installation/Konnektivität des Kennwortrückschreibens vor.
  - Es liegt ein Problem mit der Installation/Konnektivität von Azure AD Connect vor.
  - Weitere Schritte zur Problembehandlung bei Problemen mit dem Kennwortrückschreiben finden Sie unter Problembehandlung beim [Kennwortrückschreiben.](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Ich weiß nicht, wie ich das Kennwort eines Benutzers zurücksetzen kann.**

1. Melden Sie sich als entsprechender Administrator beim Azure-Portal an.
2. Wechseln Sie zum Blatt **"Benutzer und Gruppen",** und wählen **Sie "Alle Benutzer" aus.**
3. Wählen Sie einen Benutzer aus der Liste aus.
4. Wählen Sie für den ausgewählten Benutzer **"Übersicht"** und dann in der Befehlsleiste **"Kennwort zurücksetzen" aus.**
5. Wählen Sie die **Schaltfläche "Kennwort zurücksetzen"** aus, und folgen Sie den Anweisungen auf dem Bildschirm.
    - Nur Über das Azure-Portal durchgeführte **Zurücksetzungen unterstützen** das Kennwortrückschreiben.

**Ich reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**

Das Rückschreiben von Kennwörtern wird in diesem Portal nicht unterstützt. Setzen Sie das Kennwort des Benutzers im Azure-Portal erneut zurück.
