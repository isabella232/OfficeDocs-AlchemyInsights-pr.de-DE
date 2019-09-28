---
title: 2681-Angriffs Simulator in Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305331"
---
# <a name="attack-simulator-in-office-365"></a>Angriffssimulator in Office 365

- Fehlt Ihnen der Angriffs Simulator? Angriffs Simulator erfordert **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** oder **Office 365 Enterprise E5**. Der Angriffs Simulator ist **nicht** in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3 oder any Office 365 Business Subscriptions enthalten.

- Das Konto, das Sie zum Starten simulierter Angriffe verwenden, erfordert globale Administrator-oder Sicherheitsadministratorberechtigungen und mehrstufige Authentifizierung (MFA). Weitere Informationen zu Anforderungen für den Angriffs Simulator finden Sie in [diesem Thema](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Wichtige Dinge, die Sie über **Brute-Force-Kenn Wort** Angriffssimulationen wissen sollten:

  - Wenn für das Zielkonto ein MFA aktiviert ist und das Kennwort richtig erraten wurde, wird das Konto nicht als kompromittiert angezeigt (der zweite Authentifizierungs Faktor ist unvollständig).

  - Die Kennwortdatei darf nicht größer als 10 MB sein. Verwenden Sie ein Kennwort pro Zeilen, und fügen Sie eine leere Zeilen (Wagenrücklauf) nach dem letzten Kennwort in der Liste ein.

- Wichtige Dinge, die Sie über **Speer-Phishing** -Anfügungs Simulationen wissen sollten:

  - Durch Entwurf können Sie keinen benutzerdefinierten Wert für die **URL des Phishing-Anmeldeservers**angeben.

  - Wenn ein Empfänger das [Add-in "Berichtsnachricht aktivieren](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) " verwendet, um die Nachricht als Phishing zu melden, erhalten Sie möglicherweise keine Benachrichtigungen für die Nachricht (da es sich um einen simulierten Angriff handelt).

- Berichte: Wenn der simulierte Angriff abgeschlossen ist, können Sie auf **Angriffs Details** klicken, um den Bericht anzuzeigen.

- Ausführliche Anweisungen und neue Features in Attack Simulator finden Sie unter [Attack Simulator in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
