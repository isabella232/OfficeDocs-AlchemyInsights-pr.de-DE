---
title: Behandeln von Problemen bei der Registrierung von Android-Geräten in Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 0e727bd47a7d549a439e4666fa9dbb8a02e39778
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420591"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="8e37a-102">Behandeln von Problemen bei der Registrierung von Android-Geräten in Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="8e37a-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="8e37a-103">Lesen Sie die unten aufgeführten Ressourcen, um Ihr Problem jetzt zu beheben.</span><span class="sxs-lookup"><span data-stu-id="8e37a-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="8e37a-104">Einige häufige Probleme und Lösungsschritte:</span><span class="sxs-lookup"><span data-stu-id="8e37a-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="8e37a-105">**Fehler beim nicht VerschlüsselTen Gerät im Unternehmens Portal:** Neuere Versionen von Android, insbesondere ab v 7.0, erfordern einen startpasscode, um sicherzustellen, dass Ihr Gerät vollständig verschlüsselt ist.</span><span class="sxs-lookup"><span data-stu-id="8e37a-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="8e37a-106">Gängige Lösungen sind die Aktivierung einer Start-PIN oder das vollständige Verschlüsseln des Geräts.</span><span class="sxs-lookup"><span data-stu-id="8e37a-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="8e37a-107">Lesen Sie [Dieses Dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) , um weitere Informationen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="8e37a-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="8e37a-108">**Geräte können nicht mit dem InTune-Dienst Einchecken oder als "fehlerhaft" in der InTune-Verwaltungskonsole angezeigt werden:** Einige Samsung 4,4-und 5,5-Geräte können nicht in den Dienst einchecken.</span><span class="sxs-lookup"><span data-stu-id="8e37a-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="8e37a-109">Es gibt drei mögliche Lösungen für dieses Problem:</span><span class="sxs-lookup"><span data-stu-id="8e37a-109">There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="8e37a-110">Öffnen Sie die Intune-Unternehmens Portal-APP, die automatisch eine Gerätesynchronisierung initiiert.</span><span class="sxs-lookup"><span data-stu-id="8e37a-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="8e37a-111">Aktualisieren Sie das Gerät auf Android 6,0 oder höher.</span><span class="sxs-lookup"><span data-stu-id="8e37a-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="8e37a-112">Deaktivieren Sie Samsung Smart Manager aus der Verwaltung des InTune-Unternehmensportals.</span><span class="sxs-lookup"><span data-stu-id="8e37a-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="8e37a-113">Lesen Sie [Dieses Dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) , um weitere Informationen zu diesen Problemen und Lösungen zu finden.</span><span class="sxs-lookup"><span data-stu-id="8e37a-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="8e37a-114">**Benutzer lizenzTyp ungültig** oder **Benutzer Name nicht erkannt Fehler:** dem Benutzer muss eine InTune-oder EMS-Lizenz zugewiesen sein.</span><span class="sxs-lookup"><span data-stu-id="8e37a-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="8e37a-115">Lesen Sie diese Dokumente zum Zuweisen einer Lizenz über: Office Admin Center oder Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="8e37a-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="8e37a-116">Weitere Ressourcen zur Lösung des Problems:</span><span class="sxs-lookup"><span data-stu-id="8e37a-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="8e37a-117">Verwenden Sie [InTune-Problem Behandlungs Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) zur Diagnose und Lösung allgemeiner Registrierungsfehler.</span><span class="sxs-lookup"><span data-stu-id="8e37a-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="8e37a-118">Weitere Informationen finden Sie in [diesem Dokument](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="8e37a-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="8e37a-119">In [diesem Dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) finden Sie eine Liste häufig auftretender Fehler, die die Registrierung und die Auflösungen verhindern.</span><span class="sxs-lookup"><span data-stu-id="8e37a-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="8e37a-120">[Erfahren Sie, wie Sie Android-Geräte in Microsoft InTune registrieren](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="8e37a-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
    

