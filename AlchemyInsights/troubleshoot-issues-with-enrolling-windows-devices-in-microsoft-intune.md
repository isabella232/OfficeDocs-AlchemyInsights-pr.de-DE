---
title: Behandeln von Problemen bei der Registrierung von Windows-Geräten in Microsoft InTune
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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390642"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="ea812-102">Behandeln von Problemen bei der Registrierung von Windows-Geräten in Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="ea812-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="ea812-103">Lesen Sie die unten aufgeführten Ressourcen, um Ihr Problem jetzt zu beheben.</span><span class="sxs-lookup"><span data-stu-id="ea812-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="ea812-104">Einige häufige Fehlermeldungen und Lösungsschritte:</span><span class="sxs-lookup"><span data-stu-id="ea812-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="ea812-105">**Die Software kann nicht installiert werden, 0x80cf4017:** Ihr Kontozertifikat ist abgelaufen.</span><span class="sxs-lookup"><span data-stu-id="ea812-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="ea812-106">Laden Sie das PC-Client-Softwarepaket in der InTune-Verwaltungskonsole erneut herunter.</span><span class="sxs-lookup"><span data-stu-id="ea812-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="ea812-107">Weitere Informationen finden Sie in dieser Dokumentation.</span><span class="sxs-lookup"><span data-stu-id="ea812-107">Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="ea812-108">**Fehlercode 0x801c0003:** Der Fehler kann in den folgenden Szenarien auftreten:</span><span class="sxs-lookup"><span data-stu-id="ea812-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="ea812-109">Der Benutzer hat mehr Geräte als der Geräte Grenzwert registriert.</span><span class="sxs-lookup"><span data-stu-id="ea812-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="ea812-110">Lesen Sie diese Dokumente, um [ein Gerät zu entfernen](https://docs.microsoft.com/intune/devices-wipe) oder [den Geräte Grenzwert zu ändern](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="ea812-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="ea812-111">"Benutzer können Geräte mit Azure AD verbinden" ist auf "None" festgelegt.</span><span class="sxs-lookup"><span data-stu-id="ea812-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="ea812-112">Legen Sie Sie auf alle oder Benutzer auswählen fest.</span><span class="sxs-lookup"><span data-stu-id="ea812-112">Set it to all or select users.</span></span> <span data-ttu-id="ea812-113">Weitere Informationen finden Sie in [dieser Dokumentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .</span><span class="sxs-lookup"><span data-stu-id="ea812-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="ea812-114">Das Gerät ist bereits von einem anderen Benutzer registriert.</span><span class="sxs-lookup"><span data-stu-id="ea812-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="ea812-115">Wenn dies der Fall ist, entfernen Sie das Gerät aus der Azure InTune-Konsole, oder heben Sie die Registrierung des Geräts auf, bevor Sie es erneut versuchen.</span><span class="sxs-lookup"><span data-stu-id="ea812-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="ea812-116">Das Gerät ist Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="ea812-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="ea812-117">Nur Windows 10 pro, Education und Enterprise-SKUs können Azure Active Directory beitreten.</span><span class="sxs-lookup"><span data-stu-id="ea812-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="ea812-118">Weitere Ressourcen zur Lösung des Problems:</span><span class="sxs-lookup"><span data-stu-id="ea812-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="ea812-119">Verwenden Sie [InTune-Problem Behandlungs Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) zur Diagnose und Lösung allgemeiner Registrierungsfehler.</span><span class="sxs-lookup"><span data-stu-id="ea812-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="ea812-120">Weitere Informationen finden Sie in [diesem Dokument](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="ea812-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="ea812-121">Sehen Sie sich diese Dokumente an, um eine Liste allgemeiner Fehler zu finden, die die Registrierung und Auflösungen für jedes Dokument verhindern: [Problembehandlung](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) und [Problembehandlung](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="ea812-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="ea812-122">[Erfahren Sie, wie Sie Windows-Geräte in Microsoft InTune registrieren](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="ea812-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
  

