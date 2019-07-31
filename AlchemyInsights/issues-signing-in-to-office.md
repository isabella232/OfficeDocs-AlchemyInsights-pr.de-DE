---
title: Probleme bei der Anmeldung bei Office-Apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938215"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Leerer Anmeldebildschirm in Office-Apps

Um dieses Problem zu beheben, versuchen Sie Folgendes:
- Installieren Sie die neuesten Updates für [Windows](https://support.microsoft.com/help/4027667/windows-10-update) und [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Zurücksetzen Internet Explorer Optionen: Wechseln Sie zu **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (Beachten Sie, dass Sie benutzerdefinierte Einstellungen verlieren), und versuchen Sie dann erneut, sich bei Office anzumelden.
- Deaktivieren Sie den Windows Defender Application Guard (WDAG) oder eine ähnliche Firewall oder ein Antivirus-Programm:
    1. Wechseln Sie in der Systemsteuerung zu **Programme**, und wählen Sie dann **Windows-Funktionen ein-oder ausschalten aus**.
    2. Wenn der Windows Defender Application Guard aktiviert ist, deaktivieren Sie ihn.<br/>
    **Hinweis:** Möglicherweise müssen Sie den Computer neu starten.
- Stellen Sie sicher, dass das Microsoft. Aad. BrokerPlugin [Aad WAM-Plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nicht von einer Anwendung oder einem Firewall/Anti-Virus-Programm blockiert wird.
- [Löschen Sie Office-Anmeldeinformationen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) mit dem Windows-Anmelde Informations Manager.<br/>
    **Hinweis:** Die Registrierungspfade für Office 2016 haben sich in 16,0 geändert. (Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\)

Weitere Informationen finden Sie unter [Verbindungsprobleme bei der Anmeldung nach der Aktualisierung Office 2016 Build 16.0.7967 unter Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).