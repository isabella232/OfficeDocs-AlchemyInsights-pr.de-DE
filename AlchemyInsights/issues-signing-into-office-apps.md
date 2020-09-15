---
title: Probleme bei der Anmeldung bei Microsoft 365-apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695178"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Beheben von Microsoft 365-Apps "vertrauenswürdige Plattformmodul Ihres Computers funktioniert nicht ordnungsgemäß"-Meldung

Um diesen Fehler zu beheben, versuchen Sie Folgendes:

- Installieren Sie die neuesten Updates für [Windows](https://support.microsoft.com/help/4027667/windows-10-update) und [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Löschen Sie Office-Anmeldeinformationen](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) mit dem Windows-Anmelde Informations Manager.<br/>
    **Hinweis:** Die Registrierungspfade für Office 2016 haben sich in 16,0 geändert. (Beispiel: \Software\Microsoft\Office\16.0\Common\Identity\)
- Versuchen Sie den [Benutzer Wiederherstellungsprozess](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) zum Beheben von TPM-Fehlern (Trusted Platform Module).
- Legen Sie die EnableADAL = 0 mit den folgenden Schritten fest:  
    1. Klicken Sie mit der rechten Maustaste auf die Windows-Start Schaltfläche, wählen Sie **Ausführen**, geben Sie **Regedit**ein, und klicken Sie dann auf **OK**.
    2. Wählen Sie **Ja** aus, um den Registrierungs-Editor zu erlauben, Änderungen an Ihrem Gerät vorzunehmen.
    3. Fügen Sie im Registrierungs-Editor den DWORD-Wert **EnableADAL** mit der Einstellung **0** unter HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.

Weitere Informationen finden Sie unter [Verbindungsprobleme bei der Anmeldung nach der Aktualisierung Office 2016 Build 16.0.7967 unter Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).