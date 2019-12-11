---
title: Bereitstellen von Office 365 ProPlus für die gemeinsame Nutzung auf RDS, Terminal Server oder VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959459"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Bereitstellen von Office 365 ProPlus für die gemeinsame Nutzung auf RDS, Terminal Server oder VDI

So stellen Sie Office 365 ProPlus mithilfe von Remote Desktop Dienste (RDS) bereit, die früher als Terminal Dienste bezeichnet wurden:
- Sie benötigen einen Microsoft 365 for Business-Plan oder einen Office 365 Plan mit Office 365 ProPlus, beispielsweise Office 365 Enterprise E3 oder Enterprise E5.
   > [!NOTE] 
   > Die Office 365 Business-und Office 365 Business Premium-Pläne enthalten nicht Office 365 ProPlus.
- Sie müssen die [Aktivierung gemeinsam genutzter Computer](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)aktivieren.

> [!NOTE]
> Sie können den [Microsoft-Support-und Wiederherstellungs-Assistenten](https://aka.ms/SaRA_OfficeSCA_M365Portal) auch herunterladen und ausführen, um Office 365 ProPlus im Aktivierungsmodus für gemeinsam genutzte Computer zu installieren.

Weitere Informationen zu Voraussetzungen, Setupanweisungen und Anleitungen für benutzerdefinierte Installationen mithilfe des Office-Bereitstellungstools finden Sie unter [Deploy Office 365 ProPlus mithilfe von Remote Desktop Diensten](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

So beheben Sie Fehler im Zusammenhang mit der Aktivierung gemeinsam genutzter Computer:
- Weitere Informationen finden Sie unter [Beheben von Problemen mit der Aktivierung gemeinsam genutzter Computer für Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Weitere Informationen finden Sie unter [Reset Office 365 ProPlus-Aktivierungsstatus](https://go.microsoft.com/fwlink/?linkid=2109218).

Wenn Sie Office 365 ProPlus im RDS aus dem Microsoft 365 Admin Center installieren möchten, in ***dem die Standardinstallationseinstellungen verwendet***werden, führen Sie die folgenden Schritte aus:

1.  Überprüfen Sie, welche Office 365 Plan Sie haben. [Anleitung](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  Wechseln Sie bei Bedarf zu einem anderen Office 365 Plan. [Anleitung](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  Wenn Office bereits auf dem RDS-Server mit anderen Office 365 Plänen installiert ist, deinstallieren Sie es. Wenn Sie beispielsweise zur **System** > Steuerung wechseln,**deinstallieren Sie ein Programm**. Deinstallieren Sie mit dem [Microsoft-Support-und Wiederherstellungs-Assistenten,](https://aka.ms/SARA-OfficeUninstall-Alchemy) wenn Probleme auftreten.
4.  Melden Sie sich auf dem RDS-Server beim Microsoft 365 Admin Center mit Ihrem Administratorkonto an, und [Installieren Sie Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  ***Öffnen oder melden*** Sie sich nach der Installation von Office nicht bei Office-Anwendungen an.
6.  Aktivieren Sie auf dem RDS-Server die Aktivierung freigegebener Computer durch Bearbeiten der Registrierung, indem Sie die folgenden Schritte ausführen:
   1. Klicken Sie mit der rechten Maustaste auf die Windows-Schaltfläche in der unteren linken Ecke des Bildschirms, und wählen Sie **Ausführen**aus. Geben Sie im Feld Öffnen den **Befehl regedit**ein, und wählen Sie dann **OK**aus.
   2. Wählen Sie **Ja** aus, wenn Sie dazu aufgefordert werden, dass der Registrierungs-Editor Änderungen an Ihrem Gerät vorzunehmen hat.
   3. Fügen Sie im Registrierungs-Editor einen Zeichenfolgenwert von **SharedComputerLicensing** mit der Einstellung 1 unter HKEY_LOCAL_MACHINE \Software\Microsoft \Office\ClickToRun\Configuration.
   4. Melden Sie sich auf dem RDS-Server ***als Endbenutzer an*** , und [Stellen Sie sicher, dass die Aktivierung gemeinsam genutzter Computer für Office 365 ProPlus aktiviert ist](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

