---
title: Installieren von Office auf einem Terminal Server-nicht lizenziert
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 6fc4bd5f6971ca833084a6a8ad6c25b3fdafb8dc
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35381728"
---
# <a name="installing-office-on-a-terminal-server"></a>Installieren von Office auf einem Terminal Server

Für die Bereitstellung von Office 365 ProPlus auf einem Windows-Server mit Remote Desktop Diensten (RDS), ehemals Terminal Dienste genannt:
  
- Sie benötigen einen Office 365 Plan mit Office 365 ProPlus, beispielsweise Office 365 Enterprise E3 oder Enterprise E5. Die Office 365 Business-und Office 365 Business Premium-Pläne enthalten nicht Office 365 ProPlus.

- Sie müssen die [Aktivierung gemeinsam genutzter Computer](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)aktivieren.

Wenn Sie Office 365 ProPlus über das Office 365 Portal auf RDS installieren möchten, führen Sie die folgenden Schritte aus, * * in *dem die Standardinstallationseinstellungen* * * verwendet werden:
  
1. Überprüfen Sie, welche Office 365 Plan Sie haben. [Erfahren Sie, wie](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Wechseln Sie bei Bedarf zu einem anderen Office 365 Plan. [Erfahren Sie, wie](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Wenn Office bereits auf dem RDS-Server mit anderen Office 365 Plänen installiert ist, deinstallieren Sie es. Wenn Sie beispielsweise zur Systemsteuerung wechseln \> , deinstallieren Sie ein Programm. Deinstallieren Sie mit dem [Microsoft-Support-und Wiederherstellungs-Assistenten,](https://aka.ms/SARA-OfficeUninstall-Alchemy) wenn Probleme auftreten.

4. Melden Sie sich auf dem RDS-Server mit Ihrem Administratorkonto beim Office 365-Portal an, und [Installieren Sie Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. Nachdem Office installiert wurde, * * *nicht öffnen oder anmelden* * * für Office-Anwendungen.

6. Aktivieren Sie auf dem RDS-Server die Aktivierung freigegebener Computer durch Bearbeiten der Registrierung, indem Sie die folgenden Schritte ausführen:

1. Klicken Sie mit der rechten Maustaste auf die Windows-Schaltfläche in der unteren linken Ecke des Bildschirms, und wählen Sie ausführen aus. Geben Sie im Feld Öffnen den **Befehl regedit**ein, und wählen Sie dann OK aus.

2. Wählen Sie ja aus, wenn Sie dazu aufgefordert werden, dass der Registrierungs-Editor Änderungen an Ihrem Gerät vorzunehmen hat.

3. Fügen Sie im Registrierungs-Editor einen Zeichenfolgenwert von **SharedComputerLicensing** mit der Einstellung 1 unter HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Auf dem RDS-Server * * *melden* Sie sich als Endbenutzer * * an, und [Stellen Sie sicher, dass die Aktivierung gemeinsam genutzter Computer für Office 365 ProPlus aktiviert ist](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Ausführliche Informationen zu Voraussetzungen, Setupanweisungen und Anleitungen für benutzerdefinierte Installationen mithilfe des Office-Bereitstellungstools finden Sie unter [Deploy Office 365 ProPlus mithilfe von Remote Desktop Dienste](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Informationen zum Beheben von Fehlern im Zusammenhang mit der Aktivierung gemeinsam genutzter Computer finden Sie unter [Beheben von Problemen mit der Aktivierung gemeinsam genutzter Computer für Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  