---
title: Installieren von Office auf einem Terminal Server-nicht lizenziert
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 7252efdc0f55b8923e685ec89f9b3c63882aa6b0
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763216"
---
# <a name="installing-office-on-a-terminal-server"></a>Installieren von Office auf einem Terminal Server

Für die Bereitstellung von Microsoft 365-Apps für Enterprise auf einem Windows-Server mit Remote Desktop Diensten (RDS), früher benannte Terminal Dienste:
  
- Sie benötigen ein Microsoft 365-Abonnement, das Microsoft 365-Apps für Unternehmen wie Office 365 Enterprise E3 oder Enterprise E5 enthält. Die Microsoft 365 apps for Business-und Microsoft 365-Apps für Business-Premium-Pläne enthalten keine Microsoft 365-Apps für Enterprise.

- Sie müssen die [Aktivierung gemeinsam genutzter Computer](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)aktivieren.

Wenn Sie Microsoft 365-Apps für Enterprise im RDS aus dem Microsoft 365 Admin Center installieren möchten, in dem die ***Standardinstallationseinstellungen verwendet***werden, führen Sie die folgenden Schritte aus.

> [!TIP]
> Sie können den [Microsoft-Support-und Wiederherstellungs-Assistenten](https://aka.ms/SaRA_OfficeSCA_M365Portal) auch herunterladen und ausführen, um Microsoft 365-Apps für Enterprise im freigegebenen Computer Aktivierungsmodus zu installieren.
  
1. Überprüfen Sie, welches Microsoft 365-Abonnement Sie haben. [Erfahren Sie, wie](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Wechseln Sie bei Bedarf zu einem anderen Microsoft 365-Abonnement. [Erfahren Sie, wie](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Wenn Office bereits auf dem RDS-Server mit anderen Microsoft 365-Abonnements installiert ist, deinstallieren Sie es. Wenn Sie beispielsweise zur Systemsteuerung wechseln \> , deinstallieren Sie ein Programm. Deinstallieren Sie mit dem [Microsoft-Support-und Wiederherstellungs-Assistenten,](https://aka.ms/SARA-OfficeUninstall-Alchemy) wenn Probleme auftreten.

4. Melden Sie sich auf dem RDS-Server beim Microsoft 365 Admin Center mit Ihrem Administratorkonto an, und [Installieren Sie Microsoft 365 apps for Enterprise](https://portal.office.com/OLS/MySoftware.aspx).

5. ***Öffnen oder melden*** Sie sich nach der Installation von Office nicht bei Office-Anwendungen an.

6. Aktivieren Sie auf dem RDS-Server die Aktivierung freigegebener Computer durch Bearbeiten der Registrierung, indem Sie die folgenden Schritte ausführen:

1. Klicken Sie mit der rechten Maustaste auf die Windows-Schaltfläche in der unteren linken Ecke des Bildschirms, und wählen Sie ausführen aus. Geben Sie im Feld Öffnen den **Befehl regedit**ein, und wählen Sie dann OK aus.

2. Wählen Sie ja aus, wenn Sie dazu aufgefordert werden, dass der Registrierungs-Editor Änderungen an Ihrem Gerät vorzunehmen hat.

3. Fügen Sie im Registrierungs-Editor einen Zeichenfolgenwert von **SharedComputerLicensing** mit der Einstellung 1 unter HKEY_LOCAL_MACHINE \Software\Microsoft \Office\ClickToRun\Configuration.

7. Melden Sie sich auf dem RDS-Server ***als Endbenutzer an*** , und [Stellen Sie sicher, dass die Aktivierung gemeinsam genutzter Computer für Microsoft 365 apps for Enterprise aktiviert ist](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Ausführliche Informationen zu Voraussetzungen, Setupanweisungen und Anleitungen für benutzerdefinierte Installationen mithilfe des Office-Bereitstellungstools finden Sie unter [Deploy Microsoft 365 apps for Enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Informationen zum Beheben von Fehlern im Zusammenhang mit der Aktivierung gemeinsam genutzter Computer finden Sie unter [Beheben von Problemen mit der Aktivierung gemeinsam genutzter Computer für Microsoft 365 apps for Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  