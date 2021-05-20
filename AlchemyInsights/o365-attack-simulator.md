---
title: 2681 Attack Simulator in Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545725"
---
# <a name="attack-simulator-in-microsoft-365"></a>Angriffssimulator in Microsoft 365

- Fehlt Ihnen der Angriffssimulator? Der Angriffssimulator erfordert **Microsoft Defender für Office 365 Plan 2** oder Office 365 Enterprise **E5**. Der **Angriffssimulator ist** nicht in Microsoft Defender für Office 365 Plan 1, Office 365 Enterprise E3 oder in Microsoft 365 Apps for Business enthalten.

- Für das Konto, das Sie zum Starten simulierter Angriffe verwenden, sind globale Administrator- oder Sicherheitsadministratorberechtigungen und mehrstufige Authentifizierung (MFA) erforderlich. Weitere Informationen zu den Anforderungen des Angriffssimulators finden Sie [in diesem Thema.](/microsoft-365/security/office-365-security/attack-simulator)

- Wichtige Informationen zu **Brute Force Password-Angriffssimulationen:**

  - Wenn das Zielkonto MFA aktiviert hat und das Kennwort richtig erraten wurde, wird das Konto nicht als gefährdet angezeigt (der zweite Authentifizierungsfaktor ist unvollständig).

  - Die Kennwortdatei darf nicht größer als 10 MB sein. Verwenden Sie ein Kennwort pro Zeile, und fügen Sie eine leere Zeile (Wagenrücklauf) nach dem letzten Kennwort in die Liste ein.

- Wichtige Informationen zu **Spear Phishing-Anfügen-Simulationen:**

  - Standardmäßig können Sie keinen benutzerdefinierten Wert für die **Phishing-Anmeldeserver-URL angeben.**

  - Wenn ein Empfänger das [Add-In](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) Nachricht melden aktivieren verwendet, um die Nachricht als Phishing zu melden, erhalten Sie möglicherweise keine Benachrichtigungen für die Nachricht (da es sich um einen simulierten Angriff handelt).

- Berichte: Nach Abschluss des simulierten Angriffs können Sie auf **Angriffsdetails klicken,** um den Bericht anzuzeigen.

- Ausführliche Anweisungen und neue Features in Attack Simulator finden Sie unter [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).
