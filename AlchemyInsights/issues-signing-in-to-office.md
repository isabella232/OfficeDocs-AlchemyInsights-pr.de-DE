---
title: Probleme bei der Anmeldung bei Microsoft 365-Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833038"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Leerer Anmeldebildschirm in Microsoft 365-Apps

Um dieses Problem zu beheben, versuchen Sie Folgendes:
- Installieren Sie die neuesten Updates für [Windows](https://support.microsoft.com/help/4027667/windows-10-update) und [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Internet Explorer-Optionen zurücksetzen: Wechseln Sie zu **Extras**  >  **Internetoptionen**  >  **Erweiterte** Internet Explorer-Einstellungen zurücksetzen (beachten Sie, dass benutzerdefinierte Einstellungen verloren gehen), und versuchen Sie dann erneut, sich  >   bei Office zu anmelden.
- Deaktivieren Sie Windows Defender Application Guard (WDAG) oder eine ähnliche Firewall oder ein Antivirenprogramm:
    1. Wechseln Sie in der Systemsteuerung zu **Programme,** und wählen Sie dann Aktivieren oder Deaktivieren von **Windows-Features aus.**
    2. Wenn Windows Defender Application Guard aktiviert ist, versuchen Sie es zu deaktivieren.<br/>
    **Hinweis:** Möglicherweise müssen Sie den Computer neu starten.
- Stellen Sie sicher, dass das Microsoft.AAD.BrokerPlugin [AAD WAM-Plug-In](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) von keinem Anwendungsprogramm oder Firewall-/Antivirenprogramm blockiert wird.
- [Löschen von Office-Anmeldeinformationen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) mithilfe von Windows Credential Manager.<br/>
    **Hinweis:** Die Registrierungspfade für Office 2016 wurden auf 16.0 geändert. (Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\)

Weitere Informationen finden Sie unter Verbindungsprobleme bei der Anmeldung nach dem Update auf [Office 2016 Build 16.0.7967 unter Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).