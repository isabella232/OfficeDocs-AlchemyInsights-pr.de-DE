---
title: 2681-Angriffs Simulator in Microsoft 365
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
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759218"
---
# <a name="attack-simulator-in-microsoft-365"></a>Angriffs Simulator in Microsoft 365

- Fehlt Ihnen der Angriffs Simulator? Angriffs Simulator erfordert **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** oder **Office 365 Enterprise E5**. Der Angriffs Simulator ist **nicht** in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3 oder any Microsoft 365 apps for Business-Abonnements enthalten.

- Das Konto, das Sie zum Starten simulierter Angriffe verwenden, erfordert globale Administrator-oder Sicherheitsadministratorberechtigungen und mehrstufige Authentifizierung (MFA). Weitere Informationen zu Anforderungen für den Angriffs Simulator finden Sie in [diesem Thema](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Wichtige Dinge, die Sie über **Brute-Force-Kenn Wort** Angriffssimulationen wissen sollten:

  - Wenn für das Zielkonto ein MFA aktiviert ist und das Kennwort richtig erraten wurde, wird das Konto nicht als kompromittiert angezeigt (der zweite Authentifizierungs Faktor ist unvollständig).

  - Die Kennwortdatei darf nicht größer als 10 MB sein. Verwenden Sie ein Kennwort pro Zeilen, und fügen Sie eine leere Zeilen (Wagenrücklauf) nach dem letzten Kennwort in der Liste ein.

- Wichtige Dinge, die Sie über **Speer-Phishing** -Anfügungs Simulationen wissen sollten:

  - Durch Entwurf können Sie keinen benutzerdefinierten Wert für die **URL des Phishing-Anmeldeservers**angeben.

  - Wenn ein Empfänger das [Add-in "Berichtsnachricht aktivieren](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) " verwendet, um die Nachricht als Phishing zu melden, erhalten Sie möglicherweise keine Benachrichtigungen für die Nachricht (da es sich um einen simulierten Angriff handelt).

- Berichte: Wenn der simulierte Angriff abgeschlossen ist, können Sie auf **Angriffs Details** klicken, um den Bericht anzuzeigen.

- Ausführliche Anweisungen und neue Features in Attack Simulator finden Sie unter [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
