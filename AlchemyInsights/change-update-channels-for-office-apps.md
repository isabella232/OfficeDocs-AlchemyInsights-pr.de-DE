---
title: Ändern von Updatekanälen für Office-Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 3e1042a38d2289b9ef2396e8300d32f20ddaa703
ms.sourcegitcommit: b5e5f560bf6ef92b4475bd3d91b7df38b5a4b036
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/14/2020
ms.locfileid: "46739826"
---
# <a name="change-update-channels-for-office-apps"></a>Ändern von Updatekanälen für Office-Apps

Bei neuen Office-Installationen verwenden Sie die Office-Software-Downloadeinstellungen, um den gewünschten Updatekanal auszuwählen, und installieren Sie dann Office-Apps (oder installieren Sie sie erneut). Weitere Informationen finden Sie unter [Verwalten von Software-Downloadeinstellungen in Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Hinweis**: Der über die Office-Software-Downloadeinstellungen ausgewählte Updatekanal gilt für alle Benutzer, die Neuinstallationen über das O365-Portal ausführen. Weitere Informationen finden Sie unter [Herunterladen und Installieren oder erneutes Installieren von Microsoft 365 oder Office 2019 auf einem PC oder Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

Für vorhandene Office-Installationen verwenden Sie das Office-Bereitstellungstool (ODT), um zu einem anderen Updatekanal zu wechseln:  

1. Laden Sie die neueste Version des Office-Bereitstellungstools (setup.exe) aus dem [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065) herunter.
2. Identifizieren Sie den Namen des Kanals, zu dem Sie wechseln möchten. Weitere Informationen finden Sie unter [Konfigurationsoptionen für das Office-Bereitstellungstool](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Erstellen Sie eine XML-Konfigurationsdatei, und geben Sie den entsprechenden Kanalnamen an, z. B. „update.xml“.  

`<Configuration>`<br>
`<Updates Channel="Monthly"/>`<br>
`</Configuration>`<br>

4. Wechseln Sie von einer Eingabeaufforderung mit erhöhten Rechten zu dem Ordnerspeicherort, an dem sich „setup.exe“ befindet, und führen Sie den folgenden Befehl aus:  
    a. setup.exe /configure update.xml
5. Starten Sie eine Office-Anwendung (z. B. Excel), und wählen Sie dann **Datei** > **Konto** aus. Wählen Sie im Abschnitt „Produktinformationen“ **Updateoptionen** > **Jetzt aktualisieren** aus.

Weitere Informationen finden Sie unter [Wechseln von Updatekanälen für vorhandene Office-Apps](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Um Updatekanäle für eine ausgewählte Gruppe von Benutzern oder mithilfe von Configuration Manager (SCCM) zu wechseln, konfigurieren Sie die Einstellung für den Updatekanal mithilfe des Gruppenrichtlinienobjekts (GPO). Weitere Informationen finden Sie unter [Übersicht über die Updatekanäle für Microsoft 365-Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Weitere Details finden Sie unter [Verwalten von Office 365 ProPlus-Kanälen für IT-Experten](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) und [Verwalten von Updates für Microsoft 365-Apps mithilfe des Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).