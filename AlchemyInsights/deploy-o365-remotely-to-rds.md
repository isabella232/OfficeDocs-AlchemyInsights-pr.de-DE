---
title: Bereitstellen von Microsoft 365 Apps for Enterprise zur gemeinsamen Verwendung auf RDS, TerminalServer oder VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200672"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Bereitstellen von Microsoft 365 Apps for Enterprise zur gemeinsamen Verwendung auf RDS, TerminalServer oder VDI

So stellen Sie Microsoft 365 Apps for Enterprise mithilfe von Remotedesktopdiensten (Remote Desktop Services, RDS) zur Verfügung, ehemals Terminaldienste:

- Sie müssen über einen Microsoft 365 For Business-Plan oder einen Office 365-Plan verfügen, der Microsoft 365 Apps for Enterprise enthält, z. B. Office 365 Enterprise E3 oder Enterprise E5.
   > [!NOTE]
   > Die Microsoft 365 Apps for Business- und Microsoft 365 Business Standard-Pläne enthalten keine Microsoft 365 Apps for Enterprise.
- Sie müssen die Aktivierung [freigegebener Computer aktivieren.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> Sie können auch den [Microsoft Support-](https://aka.ms/SaRA_OfficeSCA_M365Portal) und Wiederherstellungs-Assistenten herunterladen und ausführen, um Microsoft 365 Apps for Enterprise im Aktivierungsmodus für gemeinsam genutzte Computer zu installieren.

Weitere Informationen zu voraussetzungen, Setupanweisungen und Anleitungen zu angepassten Installationen mithilfe des Office-Bereitstellungstools finden Sie unter [Deploy Microsoft 365 Apps for Enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

So beheben Sie Fehler im Zusammenhang mit der Aktivierung freigegebener Computer:

- Weitere [Informationen finden Sie unter Problembehandlung bei der Aktivierung freigegebener Computer für Microsoft 365 Apps for Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Siehe [Aktivierungsstatus von Microsoft 365 Apps für Unternehmen zurücksetzen](https://go.microsoft.com/fwlink/?linkid=2109218).

Wenn Sie Microsoft 365 Apps for Enterprise auf RDS aus dem Microsoft 365 Admin Center installieren ***möchten,*** das standardinstallationseinstellungen verwendet, verwenden Sie die folgenden Schritte:

1. Überprüfen Sie, welches Abonnement Sie haben. [Anleitung](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Wechseln Sie bei Bedarf zu einem anderen Abonnement. [Anleitung](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Wenn Office bereits auf dem RDS-Server mit anderen Microsoft-Abonnements installiert ist, deinstallieren Sie es. Gehen Sie z. B. zu **Systemsteuerung**  >  **Programm deinstallieren.** Deinstallieren [Sie mithilfe des Microsoft-Support-](https://aka.ms/SARA-OfficeUninstall-Alchemy) und Wiederherstellungs-Assistenten, wenn Probleme auftreten.
4. Melden Sie sich auf dem RDS-Server mit Ihrem Administratorkonto beim Microsoft 365 Admin Center an, und installieren Sie [Microsoft 365 Apps for Enterprise](https://portal.office.com/OLS/MySoftware.aspx).
5. Öffnen oder melden Sie sich nach der Installation von Office nicht ***bei*** office-Anwendungen an.
6. Aktivieren Sie auf dem RDS-Server die Aktivierung freigegebener Computer, indem Sie die Registrierung bearbeiten, indem Sie die folgenden Schritte ausführen:
   1. Klicken Sie mit der rechten Maustaste auf die Schaltfläche Windows in der unteren linken Ecke des Bildschirms, und wählen Sie **Ausführen aus.** Geben Sie regedit in das Feld **Öffnen** ein, und klicken Sie dann auf **OK**.
   2. Wählen **Sie Ja** aus, wenn Sie aufgefordert werden, dem Registrierungs-Editor das Vornehmen von Änderungen an Ihrem Gerät zu ermöglichen.
   3. Fügen Sie im Registrierungs-Editor den Zeichenfolgenwert **SharedComputerLicensing** mit der Einstellung 1 unter HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration hinzu.
   4. Melden Sie sich auf dem RDS-Server als Endbenutzer ***an,*** und vergewissern Sie sich, dass die Aktivierung gemeinsam genutzter Computer für [Microsoft 365 Apps for Enterprise aktiviert ist.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
