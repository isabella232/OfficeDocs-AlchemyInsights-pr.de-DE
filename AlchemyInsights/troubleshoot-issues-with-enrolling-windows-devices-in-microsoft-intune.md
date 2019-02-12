---
title: Behandeln von Problemen mit Windows-Geräte in Microsoft Intune registrieren
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: aa2262ed487ae4160f13490e92163a145e657862
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934775"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="61b01-102">Behandeln von Problemen mit Windows-Geräte in Microsoft Intune registrieren</span><span class="sxs-lookup"><span data-stu-id="61b01-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="61b01-103">Überprüfen Sie die unten aufgeführten Ressourcen zur Lösung des Problems jetzt.</span><span class="sxs-lookup"><span data-stu-id="61b01-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="61b01-104">Einige häufige Fehlermeldungen und Lösungsschritte:</span><span class="sxs-lookup"><span data-stu-id="61b01-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="61b01-p101">**Die Software kann nicht installiert werden, 0x80cf4017:** Ihr Kontozertifikat ist abgelaufen. Das Softwarepaket PC-Client in der Verwaltungskonsole Intune erneut herunterladen. Überprüfen Sie weitere Informationen in dieser Dokumentation.</span><span class="sxs-lookup"><span data-stu-id="61b01-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="61b01-108">**Fehlercode 0x801c0003:** Der Fehler kann in den folgenden Szenarien auftreten:</span><span class="sxs-lookup"><span data-stu-id="61b01-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="61b01-p102">Der Benutzer hat mehrere Geräte registriert Gerätegrenzwert überschreitet. Lesen Sie diese Dokumente an [ein Gerät entfernen](https://docs.microsoft.com/intune/devices-wipe) oder [Ändern Sie den Gerätegrenzwert](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="61b01-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="61b01-p103">"Benutzer Geräte Azure AD beitreten können" ist auf "none" festgelegt. Legen Sie diese auf alle oder wählen Sie Benutzer. Überprüfen Sie [in dieser Dokumentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) für Weitere Informationen.</span><span class="sxs-lookup"><span data-stu-id="61b01-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="61b01-p104">Das Gerät wird bereits von einem anderen Benutzer registriert. Wenn dies der Fall ist, entfernen Sie das Gerät aus der Konsole Azure Intune oder manuell Anmeldung kündigen Sie das Gerät, bevor Sie erneut versuchen.</span><span class="sxs-lookup"><span data-stu-id="61b01-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="61b01-p105">Das Gerät ist 10 Startseite. Nur Windows 10 Pro, Schulung und Enterprise-SKUs können Azure Active Directory teilnehmen.</span><span class="sxs-lookup"><span data-stu-id="61b01-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="61b01-118">Zusätzliche Ressourcen zu Ihrem Problem zu beheben:</span><span class="sxs-lookup"><span data-stu-id="61b01-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="61b01-p106">Mithilfe von [Intune Problembehandlung Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostizieren und Beheben von häufig auftretenden Fehler der Registrierung. Lesen Sie [Dieses Dokument](https://docs.microsoft.com/intune/help-desk-operators) für weitere Details.</span><span class="sxs-lookup"><span data-stu-id="61b01-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="61b01-121">Lesen Sie diese Dokumente für eine Liste mit häufigen Fehlern, die Registrierung und Auflösung an alle verhindern: [Handbuch für die Problembehandlung](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) und [Problembehandlung Doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="61b01-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="61b01-122">[Erfahren Sie, wie Windows-Geräte in Microsoft Intune registrieren](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="61b01-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
  

