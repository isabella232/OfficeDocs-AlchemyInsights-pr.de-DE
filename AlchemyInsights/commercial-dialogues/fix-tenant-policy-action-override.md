---
title: Beheben der Mandantenrichtlinie (Außerkraftsetzung der Aktion)
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
ms.openlocfilehash: 157baa1f1e3f48b47ba07b8c6d446f8e081a4ad24b7d48f50c4fc5af5518cdd6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896074"
---
# <a name="fix-tenant-policy-action-override"></a>Beheben der Mandantenrichtlinie (Außerkraftsetzung der Aktion)

Eine Ihrer Antispamrichtlinien wirkte sich auf diese Nachricht aus. Führen Sie die folgenden Schritte aus, um die Richtlinien zu überprüfen:

1. Wechseln Sie im Microsoft 365 Defender Portal unter <https://security.microsoft.com/> **"E-Mail & Richtlinien** für die Zusammenarbeit & Richtlinien für \>  \> **Bedrohungsregeln** \> **Antispam"** im Abschnitt **"Richtlinien".**

   Wechseln Sie direkt zur Seite **Antispamrichtlinien**, verwenden Sie <https://security.microsoft.com/antispam>.

2. Wählen Sie auf der Seite **"Antispamrichtlinien"** die Richtlinie aus, indem Sie auf den Namen der Richtlinie klicken (**Typ** ist **benutzerdefinierte Antispamrichtlinie** oder **Name** ist **Eingehende Antispamrichtlinie (Standard).**
3. Wählen Sie im angezeigten Flyout "Details" die **Option "Aktionen bearbeiten"** im Abschnitt **"Aktionen"** aus.
4. Überprüfen Sie im Abschnitt **"Nachrichtenaktionen"** die Bewertungen für **Spam,** **Spam mit hoher Spamwahrscheinlichkeit,** **Phishing** und Phishing mit **hoher Vertrauenswürdigkeit,** um festzustellen, ob einer der folgenden Werte ausgewählt ist:
   - **X-Header hinzufügen**
   - **Text in Betreffzeile voranstellen**
   - **Nachricht an E-Mail-Adresse umleiten**
   - **Nachricht löschen**
   - **Keine Aktion**

   Es ist möglich, dass die **Standardeinstellungen** auf alle Exchange Online Protection Kunden angewendet wurden, die die Nachricht betroffen haben.

Weitere Informationen finden Sie unter [Konfigurieren von Antispamrichtlinien in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
