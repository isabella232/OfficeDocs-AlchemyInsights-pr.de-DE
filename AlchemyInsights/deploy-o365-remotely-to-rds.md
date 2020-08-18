---
title: Bereitstellen von Microsoft 365-Apps für Enterprise für die gemeinsame Verwendung auf RDS, Terminal Server oder VDI
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: bd30d99221e3ddd0b07db0db78009f346babd2d0
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786276"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Bereitstellen von Microsoft 365-Apps für Enterprise für die gemeinsame Verwendung auf RDS, Terminal Server oder VDI

So stellen Sie Microsoft 365-Apps für Unternehmen mithilfe von Remote Desktop Dienste (RDS) bereit, die früher als Terminal Dienste bezeichnet wurden:
- Sie benötigen einen Microsoft 365 for Business-Plan oder einen Office 365 Plan, der Microsoft 365-Apps für Unternehmen wie Office 365 Enterprise E3 oder Enterprise E5 umfasst.
   > [!NOTE] 
   > Die Standard Pläne für Microsoft 365 apps for Business und Microsoft 365 Business Premium beinhalten keine Microsoft 365-Apps für Enterprise.
- Sie müssen die [Aktivierung gemeinsam genutzter Computer](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)aktivieren.

> [!NOTE]
> Sie können den [Microsoft-Support-und Wiederherstellungs-Assistenten](https://aka.ms/SaRA_OfficeSCA_M365Portal) auch herunterladen und ausführen, um Microsoft 365-Apps für Enterprise im freigegebenen Computer Aktivierungsmodus zu installieren.

Weitere Informationen zu Voraussetzungen, Setupanweisungen und Anleitungen für benutzerdefinierte Installationen mithilfe des Office-Bereitstellungstools finden Sie unter [Deploy Microsoft 365 apps for Enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

So beheben Sie Fehler im Zusammenhang mit der Aktivierung gemeinsam genutzter Computer:
- Weitere Informationen finden Sie unter [Beheben von Problemen mit der Aktivierung gemeinsam genutzter Computer für Microsoft 365 apps for Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Siehe [Aktivierungsstatus von Microsoft 365 Apps für Unternehmen zurücksetzen](https://go.microsoft.com/fwlink/?linkid=2109218).

Wenn Sie Microsoft 365-Apps für Enterprise im RDS aus dem Microsoft 365 Admin Center installieren möchten, in ***dem die Standardinstallationseinstellungen verwendet***werden, führen Sie die folgenden Schritte aus:

1.    Überprüfen Sie, welches Abonnement Sie haben. [Anleitung](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Wechseln Sie bei Bedarf zu einem anderen Abonnement. [Anleitung](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Wenn Office bereits auf dem RDS-Server mit anderen Microsoft-Abonnements installiert ist, deinstallieren Sie es. Wenn Sie beispielsweise zur **System**Steuerung wechseln,  >  **deinstallieren Sie ein Programm**. Deinstallieren Sie mit dem [Microsoft-Support-und Wiederherstellungs-Assistenten,](https://aka.ms/SARA-OfficeUninstall-Alchemy) wenn Probleme auftreten.
4.    Melden Sie sich auf dem RDS-Server beim Microsoft 365 Admin Center mit Ihrem Administratorkonto an, und [Installieren Sie Microsoft 365 apps for Enterprise](https://portal.office.com/OLS/MySoftware.aspx).
5.    ***Öffnen oder melden*** Sie sich nach der Installation von Office nicht bei Office-Anwendungen an.
6.    Aktivieren Sie auf dem RDS-Server die Aktivierung freigegebener Computer durch Bearbeiten der Registrierung, indem Sie die folgenden Schritte ausführen:
   1. Klicken Sie mit der rechten Maustaste auf die Windows-Schaltfläche in der unteren linken Ecke des Bildschirms, und wählen Sie **Ausführen**aus. Geben Sie im Feld Öffnen den **Befehl regedit**ein, und wählen Sie dann **OK**aus.
   2. Wählen Sie **Ja** aus, wenn Sie dazu aufgefordert werden, dass der Registrierungs-Editor Änderungen an Ihrem Gerät vorzunehmen hat.
   3. Fügen Sie im Registrierungs-Editor einen Zeichenfolgenwert von **SharedComputerLicensing** mit der Einstellung 1 unter HKEY_LOCAL_MACHINE \Software\Microsoft \Office\ClickToRun\Configuration.
   4. Melden Sie sich auf dem RDS-Server ***als Endbenutzer an*** , und [Stellen Sie sicher, dass die Aktivierung gemeinsam genutzter Computer für Microsoft 365 apps for Enterprise aktiviert ist](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

