---
title: Kennwortsynchronisierung
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449140"
---
# <a name="password-synchronization"></a>Kennwortsynchronisierung

**Kennworthashsynchronisierung funktioniert überhaupt nicht**

Einige häufige Probleme, die Kunden auftreten, wenn die Kennworthashsynchronisierung nicht funktioniert, sind:

- Das active Directory-Konto, das von Azure AD Connect für  die Kommunikation mit lokalem Active Directory verwendet wird, erhält keine Replikation von Verzeichnisänderungen und Verzeichnisänderungen **Replizieren Alle** Berechtigungen, die für die Kennwortsynchronisierung erforderlich sind. Sie müssen dies beheben, indem Sie dem Active Directory-Konto diese Berechtigungen erteilen.
- Die Kennworthashsynchronisierung wird deaktiviert, nachdem ein  Administrator die User Sign-In-Methode von der Kennwortsynchronisierung in eine andere Option wie  den Verbund mit **AD FS** im Azure AD Sign-In geändert hat. Sie können dies beheben, indem Sie das Feature für die Kennworthashsynchronisierung im Azure AD #A1 erneut aktivieren.
- Verbindungsproblem mit lokalem Active Directory. Beispielsweise kann azure AD Connect nicht auf einige [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) Domänencontroller zugreifen, oder die erforderlichen Ports werden von der Firewall blockiert. Sie müssen dies beheben, indem Sie sicherstellen, dass die Verbindung zwischen dem Azure AD Connect-Server und dem lokalen Active Directory ordnungsgemäß funktioniert.
- Azure AD #A0 befindet sich derzeit im Stagingmodus, was dazu führt, dass der Server nicht in der Lage ist, die Kennworthashes zu verwenden. Führen Sie zur Problembehandlung die im Abschnitt Problembehandlung bei der Kennwortsynchronisierung mit azure AD Connect-Synchronisierung beschriebenen Schritte aus: Keine Kennwörter werden [synchronisiert.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

**Kennworthashsynchronisierung funktioniert für einige meiner Benutzer nicht**

1. Wenn Sie festgestellt haben, dass der Kennworthash  für einen Benutzer nicht synchronisiert wird, verwenden Sie die Problembehandlungsaufgabe in Azure AD Connect, um das Problem zu untersuchen und zu beheben. Führen Sie die folgenden Aufgaben aus:

    a. [Ausführen der Problembehandlungsaufgabe im Assistenten](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Verwenden des Cmdlets zur Problembehandlung, um das Problem der Kennworthashsynchronisierung für eine bestimmte Verwendung zu untersuchen](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Das lokale Active Directory User-Objekt ist für Benutzer aktiviert, um das Kennwort bei der **nächsten Anmeldeoption zu** ändern. Wenn diese Option aktiviert ist, wird dem Benutzer ein temporäres Kennwort zugewiesen, und er wird aufgefordert, das Kennwort bei der nächsten Anmeldung zu ändern. Azure AD Connect synchronisiert keine temporären Kennwörter mit Azure AD.

Führen Sie eine der folgenden Aufgaben aus, um das oben beschriebene Problem zu beheben:

- Bitten Sie den Benutzer, sich bei der lokalen Anwendung (z. B. Windows Desktop) zu anmelden und das Kennwort zu ändern. Das neue Kennwort wird mit Azure AD synchronisiert.
- Ein Administrator muss das Kennwort des Benutzers aktualisieren, ohne die Option Benutzer muss das Kennwort bei der nächsten Anmeldung ändern **und** das neue Kennwort für den Benutzer freigeben.

3. Das lokale Active Directory User-Objekt ist **nicht ordnungsgemäß** für die Objektsynchronisierung oder Kennwortsynchronisierung konfiguriert. Um dieses Problem zu beheben, führen Sie die unter Problembehandlung der Kennworthashsynchronisierung mit [Azure AD Connect-Synchronisierung](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)beschriebenen Schritte aus.







