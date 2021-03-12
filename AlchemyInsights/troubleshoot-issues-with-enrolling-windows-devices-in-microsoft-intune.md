---
title: Behandeln von Problemen bei der Registrierung von Windows-Geräten in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708889"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Behandeln von Problemen bei der Registrierung von Windows-Geräten in Microsoft Intune

Überprüfen Sie die unten aufgeführten Ressourcen, um Ihr Problem jetzt zu beheben.
  
Einige häufige Fehlermeldungen und Lösungsschritte:
  
 **Die Software kann nicht installiert werden, 0x80cf4017:** Ihr Kontozertifikat ist abgelaufen. Laden Sie das PC-Client-Softwarepaket erneut in der Intune Admin Console herunter. Weitere Informationen finden Sie in dieser Dokumentation.
  
 **Fehlercode 0x801c0003:** Der Fehler kann in den folgenden Szenarien auftreten:
  
-  Der Benutzer hat mehr Geräte als das Gerätelimit registriert. Überprüfen Sie diese Dokumente, [um ein Gerät zu entfernen oder](https://docs.microsoft.com/intune/devices-wipe) das [Gerätelimit zu ändern.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "Benutzer können Geräte zu Azure AD beitreten" ist auf "keine" festgelegt. Legen Sie es auf alle Benutzer oder wählen Sie Benutzer aus. Weitere [Informationen finden](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) Sie in dieser Dokumentation.

-  Das Gerät wurde bereits von einem anderen Benutzer registriert. Wenn dies der Fall ist, entfernen Sie das Gerät aus der Azure Intune-Konsole, oder entrollen Sie das Gerät manuell, bevor Sie es erneut versuchen.

-  Das Gerät ist Windows 10 Home. Nur Windows 10 Pro-, Education- und Enterprise-SKUs können Azure Active Directory beitreten.

Zusätzliche Ressourcen zur Lösung Ihres Problems:
  
-  Verwenden [Sie das Intune-Problembehandlungsportal,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) um häufige Registrierungsfehler zu diagnostizieren und zu beheben. Weitere [Informationen finden](https://docs.microsoft.com/intune/help-desk-operators) Sie in diesem Dokument.

-  Sehen Sie sich diese Dokumente an, um eine Liste häufig auftretender Fehler, die die Registrierung verhindern, sowie Lösungen dafür zu finden: [Anleitung zur Problembehandlung](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) und [Problembehandlungsdokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Erfahren Sie, wie Sie Windows-Geräte in Microsoft Intune registrieren.](https://docs.microsoft.com/intune/windows-enroll)
