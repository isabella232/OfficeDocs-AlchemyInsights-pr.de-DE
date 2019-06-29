---
title: Behandeln von Problemen beim Registrieren von Android-Geräten in Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 9cdfda0d7dd45af260f46738cbc85aac46f53960
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35367288"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="ce042-102">Behandeln von Problemen beim Registrieren von Android-Geräten in Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="ce042-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="ce042-103">Überprüfen Sie die unten aufgeführten Ressourcen, um Ihr Problem jetzt zu beheben.</span><span class="sxs-lookup"><span data-stu-id="ce042-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="ce042-104">Einige häufige Probleme und Lösungsschritte:</span><span class="sxs-lookup"><span data-stu-id="ce042-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="ce042-105">**Fehler des nicht verschlüsselten Geräts im Unternehmens Portal:** Neuere Versionen von Android, insbesondere ab v 7.0, erfordern eine Startkennung, um sicherzustellen, dass Ihr Gerät vollständig verschlüsselt ist.</span><span class="sxs-lookup"><span data-stu-id="ce042-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="ce042-106">Häufige Lösungen sind das Aktivieren einer Start-PIN oder das vollständige Verschlüsseln des Geräts.</span><span class="sxs-lookup"><span data-stu-id="ce042-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="ce042-107">Lesen Sie [Dieses Dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) , um weitere Informationen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="ce042-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="ce042-108">**Geräte können nicht mit dem InTune-Dienst Einchecken oder in der InTune-Verwaltungskonsole als "ungesund" anzeigen:** Einige Geräte von Samsung 4,4 und 5,5 werden möglicherweise nicht in den Dienst eingecheckt.</span><span class="sxs-lookup"><span data-stu-id="ce042-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="ce042-109">Es gibt drei mögliche Lösungen für dieses Problem:</span><span class="sxs-lookup"><span data-stu-id="ce042-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="ce042-110">Öffnen Sie die Intune-Unternehmens Portal-app manuell, wodurch automatisch eine Gerätesynchronisierung initiiert wird.</span><span class="sxs-lookup"><span data-stu-id="ce042-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="ce042-111">Aktualisieren Sie das Gerät auf Android 6,0 oder höher.</span><span class="sxs-lookup"><span data-stu-id="ce042-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="ce042-112">Deaktivieren Sie Samsung Smart Manager für die Verwaltung des InTune-Unternehmensportals.</span><span class="sxs-lookup"><span data-stu-id="ce042-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="ce042-113">Lesen Sie [Dieses Dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) , um weitere Details zu diesen Problemen und Lösungen zu erfahren.</span><span class="sxs-lookup"><span data-stu-id="ce042-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="ce042-114">Der **Benutzer Lizenztyp ist ungültig** oder der **Benutzer Name wurde nicht erkannt Fehler:** dem Benutzer muss eine InTune-oder EMS-Lizenz zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="ce042-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="ce042-115">Überprüfen Sie diese Dokumente zum Zuweisen einer Lizenz über: Office Admin Center oder Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="ce042-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="ce042-116">Zusätzliche Ressourcen zur Lösung Ihres Problems:</span><span class="sxs-lookup"><span data-stu-id="ce042-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="ce042-117">Verwenden Sie das [InTune-Problem Behandlungs Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , um häufige Registrierungsfehler zu diagnostizieren und zu beheben.</span><span class="sxs-lookup"><span data-stu-id="ce042-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="ce042-118">Lesen Sie [Dieses Dokument](https://docs.microsoft.com/intune/help-desk-operators) , um weitere Details zu erfahren.</span><span class="sxs-lookup"><span data-stu-id="ce042-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="ce042-119">Lesen Sie [Dieses Dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) , um eine Liste der häufigsten Fehler zu finden, die die Registrierung und Auflösungen verhindern.</span><span class="sxs-lookup"><span data-stu-id="ce042-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="ce042-120">[Erfahren Sie, wie Sie Android-Geräte in Microsoft InTune registrieren](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="ce042-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
