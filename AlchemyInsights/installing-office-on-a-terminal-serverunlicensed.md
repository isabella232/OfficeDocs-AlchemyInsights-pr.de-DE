---
title: Installieren von Office auf einem Terminalserver - nicht lizenzierten
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29470065"
---
# <a name="installing-office-on-a-terminal-server"></a>Installieren von Office auf einem Terminalserver

Für die Bereitstellung von Office 365 ProPlus auf einem Windows-Server mit Remote Desktop Services (RDS), namens früher Terminaldienste:
  
- Sie müssen einen Office 365-Plan verfügen, der Office 365 ProPlus, wie Office 365 Enterprise E3 oder Enterprise E5 enthält. Die Office 365 Geschäfts- und Office 365 Business Premium Pläne enthalten nicht Office 365 ProPlus.
    
- Sie müssen [gemeinsam genutzter Computer Aktivierung](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)zu aktivieren.
    
Wenn Sie Office 365 ProPlus über das Office 365-Portal auf RDS installieren möchten ** *die Standardeinstellungen für die Installation verwendet* **, gehen Sie folgendermaßen vor: 
  
1. Welche Office 365-Plan Sie haben überprüfen. [Erfahren Sie, wie](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. Falls erforderlich, wechseln Sie zu einem anderen Office 365 planen. [Erfahren Sie, wie](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. Wenn Office bereits auf dem anderen Office 365-Pläne mit RDS-Server installiert ist, deinstallieren Sie es. Angenommen, indem Sie auf Systemsteuerung \> Programm deinstallieren. Deinstallieren Sie [Microsoft-Support und Recovery-Assistenten](https://aka.ms/SARA-OfficeUninstall-Alchemy) verwenden, wenn Sie Probleme ausführen. 
    
4. Melden Sie sich auf dem Server RDS in Office 365-Portal mit Ihrem Administratorkonto und [Installieren von Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)an.
    
5. Nach der Installation von Office ** *Öffnen oder melden Sie sich nicht* ** für alle Office-Clientanwendungen. 
    
6. Aktivieren Sie auf dem Server RDS gemeinsam genutzter Computer Aktivierung durch Bearbeiten der Registrierung durch die folgenden Schritte ausführen:
    
1. Mit der rechten Maustaste in der unteren linken Ecke des Bildschirms der Windows-Schaltfläche, und wählen Sie ausführen aus. Öffnen Sie im Feld Geben Sie **regedit ein**, und wählen Sie dann auf OK. 
    
2. Wählen Sie Ja bei entsprechender Aufforderung zum Zulassen des Registrierungs-Editor auf Ihrem Gerät ändern.
    
3. In den Registrierungs-Editor, fügen einen String-Wert der **SharedComputerLicensing** mit der Einstellung 1 unter HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration hinzu. 
    
7. Auf dem Server RDS ** *Melden Sie sich als Endbenutzer* ** und [Stellen Sie sicher, dass gemeinsam genutzter Computer Aktivierung für Office 365 ProPlus aktiviert ist](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
Weitere Informationen zu Voraussetzungen, zur Einrichtung und Anleitungen für benutzerdefinierte Installationen mithilfe des Office-Bereitstellungstools Bitte finden Sie unter [Bereitstellen von Office 365 ProPlus mithilfe von Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Zum Beheben von Fehlern im Zusammenhang mit der Aktivierung des freigegebenen finden Sie unter [Troubleshoot Probleme bei der Aktivierung für Office 365 ProPlus gemeinsam genutzter Computer](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  

