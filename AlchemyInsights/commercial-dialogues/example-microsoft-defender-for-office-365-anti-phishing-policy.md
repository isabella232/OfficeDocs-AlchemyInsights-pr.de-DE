---
title: Beispiel für Microsoft Defender für Office 365-Antiphishingrichtlinie
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737184"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Beispiel für Microsoft Defender für Office 365-Antiphishingrichtlinie

Mit diesen Einstellungen wird eine Richtlinie namens *"Domäne und CEO" aktiviert.* Diese Richtlinie bietet Sowohl Benutzer- als auch Domänenschutz vor Identitätswechseln und wendet die Richtlinie dann auf alle E-Mails an, die von Benutzern innerhalb der Domäne empfangen werden. Fügen Sie zunächst die folgenden Informationen hinzu, um die Richtlinie zu erstellen:

- **Name**: Domänen- und **CEO-Beschreibung**: Stellt sicher, dass der CEO und Ihre Domäne nicht als identitätswechselt werden.
  **Angewendet auf**: Select **Die Empfängerdomäne ist**. Wählen **Sie unter Alle diese** Die Option **Auswählen** aus, und wählen Sie dann eine Domäne aus. Wählen Sie **+ Hinzufügen** aus. Aktivieren Sie das Kontrollkästchen neben dem Namen der Domäne in der Liste (z. B. contoso.com *),* und wählen Sie dann **Hinzufügen aus.** Wählen Sie **Fertig** aus.
- Nachdem die Richtlinie erstellt wurde, können Sie die Richtlinie mithilfe der folgenden Optionen optimieren:
  - **Hinzufügen von Benutzern zum Schützen:** Fügen Sie in diesem Beispiel mindestens die E-Mail-Adresse des CEO hinzu.
  - **Zu schützende** Domänen hinzufügen: Fügen Sie die Organisationsdomäne hinzu, die das Büro des CEO enthält.
  - **Aktionen auswählen:** Wenn E-Mails von einem identitätswechselten Benutzer gesendet **werden,** wählen Sie **Nachricht** an eine andere E-Mail-Adresse umleiten aus, und geben Sie dann die E-Mail-Adresse des Sicherheitsadministrators ein (z. B. *securityadmin@contoso.com*). For **If email is sent by an impersonated domain,** select Quarantine the **message**.
  - **Postfachintelligenz:** Diese Option ist standardmäßig ausgewählt, wenn Sie eine neue Antiphishingrichtlinie erstellen. Lassen Sie diese Einstellung auf **Ein**, um optimale Ergebnisse zu erzielen.
  - **Hinzufügen vertrauenswürdiger Absender und Domänen:** Definieren Sie in diesem Beispiel keine Außerkraftsetzungen.
- Nachdem Sie Ihre Einstellungen überprüft haben, wählen Sie Diese Richtlinie **erstellen** oder **Speichern** aus.

Weitere Informationen finden Sie unter [Antiphishingrichtlinien in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
