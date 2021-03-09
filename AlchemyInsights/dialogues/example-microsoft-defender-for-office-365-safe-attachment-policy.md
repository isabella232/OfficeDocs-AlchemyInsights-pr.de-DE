---
title: Beispiel für microsoft defender for Office 365 Safe Attachment policy
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50530077"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Beispiel für microsoft defender for Office 365 Safe Attachment policy

Mit diesen Einstellungen wird eine Richtlinie namens *Keine* Verzögerungen aktiviert, die Nachrichten sofort übermittelt und anlagen nach dem Scannen erneut angibt:

- **Name**: Keine Verzögerungen
- **Beschreibung**: Übermittelt Nachrichten sofort und legt Anlagen nach dem Scannen erneut an.
- **Antwort**: Wählen Sie die **Option Dynamische Zustellung** aus. Weitere Informationen finden Sie unter [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).
- **Abschnitt** Umleitungsanlage: Wählen Sie die Option Umleitung aktivieren **aus,** und geben Sie dann die E-Mail-Adresse Ihres globalen Microsoft 365-Administrators, Sicherheitsadministrators oder Sicherheitsanalysten ein, der schädliche Anlagen untersuchen wird.
- **Abschnitt Angewendet auf:** Wählen Sie **Die Empfängerdomäne ist**, und wählen Sie dann Ihre Domäne aus. Wählen **Sie Hinzufügen** aus, und wählen Sie dann OK **aus.** Nachdem Sie fertig sind, wählen Sie **Speichern aus.**

Weitere Informationen finden Sie unter [Sichere Anlagen in Microsoft Defender für Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).
