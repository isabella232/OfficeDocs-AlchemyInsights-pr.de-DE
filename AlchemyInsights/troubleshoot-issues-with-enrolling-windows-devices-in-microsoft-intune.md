---
title: Behandeln von Problemen mit Windows-Geräte in Microsoft Intune registrieren
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28289996"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Behandeln von Problemen mit Windows-Geräte in Microsoft Intune registrieren

Überprüfen Sie die unten aufgeführten Ressourcen zur Lösung des Problems jetzt. 
  
Einige häufige Fehlermeldungen und Lösungsschritte:
  
 **Die Software kann nicht installiert werden, 0x80cf4017:** Ihr Kontozertifikat ist abgelaufen. Das Softwarepaket PC-Client in der Verwaltungskonsole Intune erneut herunterladen. Überprüfen Sie weitere Informationen in dieser Dokumentation. 
  
 **Fehlercode 0x801c0003:** Der Fehler kann in den folgenden Szenarien auftreten: 
  
1. Der Benutzer hat mehrere Geräte registriert Gerätegrenzwert überschreitet. Lesen Sie diese Dokumente an [ein Gerät entfernen](https://docs.microsoft.com/en-us/intune/devices-wipe) oder [Ändern Sie den Gerätegrenzwert](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. "Benutzer Geräte Azure AD beitreten können" ist auf "none" festgelegt. Legen Sie diese auf alle oder wählen Sie Benutzer. Überprüfen Sie [in dieser Dokumentation](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) für Weitere Informationen. 
    
3. Das Gerät wird bereits von einem anderen Benutzer registriert. Wenn dies der Fall ist, entfernen Sie das Gerät aus der Konsole Azure Intune oder manuell Anmeldung kündigen Sie das Gerät, bevor Sie erneut versuchen.
    
4. Das Gerät ist 10 Startseite. Nur Windows 10 Pro, Schulung und Enterprise-SKUs können Azure Active Directory teilnehmen.
    
Zusätzliche Ressourcen zu Ihrem Problem zu beheben:
  
1. Mithilfe von [Intune Problembehandlung Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostizieren und Beheben von häufig auftretenden Fehler der Registrierung. Lesen Sie [Dieses Dokument](https://docs.microsoft.com/en-us/intune/help-desk-operators) für weitere Details. 
    
2. Lesen Sie diese Dokumente für eine Liste mit häufigen Fehlern, die Registrierung und Auflösung an alle verhindern: [Handbuch für die Problembehandlung](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) und [Problembehandlung Doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Erfahren Sie, wie Windows-Geräte in Microsoft Intune registrieren](https://docs.microsoft.com/en-us/intune/windows-enroll).
  

