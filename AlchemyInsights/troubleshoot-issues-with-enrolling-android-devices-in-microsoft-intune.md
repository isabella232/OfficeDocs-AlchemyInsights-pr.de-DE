---
title: Behandeln von Problemen mit Android-Geräte in Microsoft Intune registrieren
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 2f4fc434128ebe7323f0b8c08aec3be82112bbda
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28290267"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="70a73-102">Behandeln von Problemen mit Android-Geräte in Microsoft Intune registrieren</span><span class="sxs-lookup"><span data-stu-id="70a73-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="70a73-103">Überprüfen Sie die unten aufgeführten Ressourcen zur Lösung des Problems jetzt.</span><span class="sxs-lookup"><span data-stu-id="70a73-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="70a73-104">Häufige Probleme und Lösungsschritte:</span><span class="sxs-lookup"><span data-stu-id="70a73-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="70a73-p101">**Gerät nicht verschlüsselt Fehler im Unternehmensportal:** Sobald neuere Versionen von Android, insbesondere beginnend mit Version 7.0, erforderlich zum Starten des Kennung dafür sorgen, dass Ihr Gerät vollständig verschlüsselt ist. Häufig sind, aktivieren eine Pin zum Starten des oder das Gerät vollständig zu verschlüsseln. Lesen Sie [Dieses Dokument](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) Weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="70a73-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="70a73-p102">**Nicht Geräten erkundigen Sie sich bei dem Intune-Dienst oder als "Fehlerhaft" in der Verwaltungskonsole Intune anzeigen:** Einige Samsung 4.4 und 5.5 Geräte möglicherweise nicht in den Dienst überprüft. Es gibt 3 Lösungsvorschläge für dieses Problem:</span><span class="sxs-lookup"><span data-stu-id="70a73-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="70a73-110">Öffnen Sie manuell die Intune Unternehmensportal-app, die automatisch eine Synchronisierung Gerät wird initiiert.</span><span class="sxs-lookup"><span data-stu-id="70a73-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="70a73-111">Aktualisieren Sie das Gerät auf Android 6.0 oder höher.</span><span class="sxs-lookup"><span data-stu-id="70a73-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="70a73-p103">Verwalten von der Intune Unternehmensportal deaktivieren Sie Samsung Smart-Manager. [In diesem Dokument](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) Weitere Informationen zu diesen Problemen und Lösungen überprüfen.</span><span class="sxs-lookup"><span data-stu-id="70a73-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="70a73-p104">**Benutzer Lizenz Typ ungültig** oder **Fehler Benutzer Name nicht erkannt:** der Benutzer eine Lizenz Intune oder zur Abstimmung zugewiesen werden soll. Lesen Sie diese Dokumente über eine Lizenz zuweisen: Office-Verwaltungskonsole oder Azure-Portal.</span><span class="sxs-lookup"><span data-stu-id="70a73-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="70a73-116">Zusätzliche Ressourcen zu Ihrem Problem zu beheben:</span><span class="sxs-lookup"><span data-stu-id="70a73-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="70a73-p105">Mithilfe von [Intune Problembehandlung Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostizieren und Beheben von häufig auftretenden Fehler der Registrierung. Lesen Sie [Dieses Dokument](https://docs.microsoft.com/en-us/intune/help-desk-operators) für weitere Details.</span><span class="sxs-lookup"><span data-stu-id="70a73-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="70a73-119">Lesen Sie [Dieses Dokument](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) für eine Liste mit häufigen Fehlern, die Registrierung und Auflösung für jeden zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="70a73-119">Review [this document](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="70a73-120">[Erfahren Sie, wie in Microsoft Intune Android-Geräte zu registrieren](https://docs.microsoft.com/en-us/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="70a73-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/android-enroll).</span></span>
    

