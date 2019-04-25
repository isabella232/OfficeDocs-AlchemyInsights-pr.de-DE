---
title: Installieren von Office auf einem Terminal Server – nicht lizenziert
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 971edd9c064b448446ba16361e99df4a2291c14f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32410121"
---
# <a name="installing-office-on-a-terminal-server"></a>Installieren von Office auf einem Terminal Server

Für die Bereitstellung von Office 365 proPlus auf einem Windows-Server mit Remote Desktop Dienste (RDS), früher als Terminal Dienste bezeichnet:
  
- Sie benötigen einen Office 365-Plan mit Office 365 proPlus, wie Office 365 Enterprise E3 oder Enterprise E5. Die Office 365 Business-und Office 365 Business Premium-Pläne schließen nicht Office 365 proPlus aus.
    
- Sie müssen die [Aktivierung gemeinsam genutzter Computer](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)aktivieren.
    
Führen Sie die folgenden Schritte aus, wenn Sie Office 365 proPlus auf RDS aus dem Office 365-Portal installieren möchten, * * *das Standardinstallationseinstellungen* * * verwendet: 
  
1. Überprüfen Sie, welche Office 365-Plan Sie haben. [Erfahren Sie, wie](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. Wechseln Sie gegebenenfalls zu einem anderen Office 365-Plan. [Erfahren Sie, wie](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. Wenn Office bereits auf dem RDS-Server mit anderen Office 365-Plänen installiert ist, deinstallieren Sie es. Beispielsweise \> deinstallieren Sie ein Programm in der Systemsteuerung. Deinstallieren Sie mit [Microsoft-Support und Wiederherstellungs-Assistent,](https://aka.ms/SARA-OfficeUninstall-Alchemy) wenn Probleme auftreten. 
    
4. Melden Sie sich auf dem RDS-Server im Office 365-Portal mit Ihrem Administratorkonto an, und [Installieren Sie Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
    
5. Nach der Installation von Office, * * *Öffnen Sie nicht oder melden* Sie * * für Office-Anwendungen an. 
    
6. Aktivieren Sie auf dem RDS-Server die Aktivierung gemeinsam genutzter Computer durch Bearbeiten der Registrierung, indem Sie die folgenden Schritte ausführen:
    
1. Klicken Sie mit der rechten Maustaste in der unteren linken Ecke des Bildschirms auf die Schaltfläche Windows, und wählen Sie ausführen aus. Geben Sie im Feld Öffnen den **Befehl regedit**ein, und wählen Sie dann OK aus. 
    
2. Wählen Sie ja aus, wenn Sie dazu aufgefordert werden, den Registrierungs-Editor zu ändern.
    
3. Fügen Sie im Registrierungs-Editor einen Zeichenfolgenwert von **SharedComputerLicensing** mit der Einstellung 1 unter HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 
    
7. Auf dem RDS-Server * * *melden* Sie sich als Endbenutzer * * an, und [Stellen Sie sicher, dass die Aktivierung gemeinsam genutzter computer für Office 365 ProPlus aktiviert ist](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
Weitere Informationen zu den Voraussetzungen, Setupanweisungen und Anleitungen für angepasste Installationen mithilfe des Office-BereitstellungsTools finden Sie unter [Deploy office 365 ProPlus mithilfe der Remote Desktop Dienste](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Informationen zur Behebung von Fehlern im Zusammenhang mit der Aktivierung gemeinsam genutzter Computer finden Sie unter [Beheben von Problemen mit der Aktivierung gemeinsam genutzter Computer für Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  

