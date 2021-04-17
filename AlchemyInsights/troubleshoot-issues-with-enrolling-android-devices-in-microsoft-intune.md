---
title: Behandeln von Problemen bei der Registrierung von Android-Geräten in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830941"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="36f27-102">Behandeln von Problemen bei der Registrierung von Android-Geräten in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="36f27-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="36f27-103">Überprüfen Sie die unten aufgeführten Ressourcen, um Ihr Problem jetzt zu beheben.</span><span class="sxs-lookup"><span data-stu-id="36f27-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="36f27-104">Einige häufige Probleme und Lösungsschritte:</span><span class="sxs-lookup"><span data-stu-id="36f27-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="36f27-105">**Fehler "Gerät nicht verschlüsselt" im Unternehmensportal:** Neuere Versionen von Android, insbesondere ab v7.0, erfordern eine Startkennung, um sicherzustellen, dass Ihr Gerät vollständig verschlüsselt ist.</span><span class="sxs-lookup"><span data-stu-id="36f27-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="36f27-106">Häufige Lösungen sind das Aktivieren eines Startpins oder das vollständige Verschlüsseln des Geräts.</span><span class="sxs-lookup"><span data-stu-id="36f27-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="36f27-107">Weitere [Informationen finden](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) Sie in diesem Dokument.</span><span class="sxs-lookup"><span data-stu-id="36f27-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="36f27-108">Geräte können nicht mit dem Intune-Dienst einchecken oder in der Intune-Verwaltungskonsole als **"Fehlerhaft" anzeigen:** Einige Geräte von Samsung 4.4 und 5.5 checken möglicherweise nicht in den Dienst ein.</span><span class="sxs-lookup"><span data-stu-id="36f27-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="36f27-109">Es gibt 3 mögliche Lösungen für dieses Problem:</span><span class="sxs-lookup"><span data-stu-id="36f27-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="36f27-110">Öffnen Sie manuell die Intune Company Portal-App, die automatisch eine Gerätesynchronisierung initiiert.</span><span class="sxs-lookup"><span data-stu-id="36f27-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="36f27-111">Aktualisieren Sie das Gerät auf Android 6.0 oder höher.</span><span class="sxs-lookup"><span data-stu-id="36f27-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="36f27-112">Deaktivieren Sie den Samsung Smart Manager von der Verwaltung des Intune-Unternehmensportals.</span><span class="sxs-lookup"><span data-stu-id="36f27-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="36f27-113">Weitere [Informationen zu](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) diesen Problemen und Lösungen finden Sie in diesem Dokument.</span><span class="sxs-lookup"><span data-stu-id="36f27-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="36f27-114">**Fehler "Benutzerlizenztyp Ungültig"** oder "Benutzername **nicht erkannt":** Dem Benutzer muss eine Intune- oder EMS-Lizenz zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="36f27-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="36f27-115">Überprüfen Sie diese Dokumente, um eine Lizenz zuzuordnen: Office Admin Center oder Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="36f27-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="36f27-116">Zusätzliche Ressourcen zur Lösung Ihres Problems:</span><span class="sxs-lookup"><span data-stu-id="36f27-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="36f27-117">Verwenden [Sie das Intune-Problembehandlungsportal,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) um häufige Registrierungsfehler zu diagnostizieren und zu beheben.</span><span class="sxs-lookup"><span data-stu-id="36f27-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="36f27-118">Weitere [Informationen finden](https://docs.microsoft.com/intune/help-desk-operators) Sie in diesem Dokument.</span><span class="sxs-lookup"><span data-stu-id="36f27-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="36f27-119">In [diesem Dokument finden](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) Sie eine Liste der häufigen Fehler, die die Registrierung und Die Lösung der einzelnen Fehler verhindern.</span><span class="sxs-lookup"><span data-stu-id="36f27-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="36f27-120">[Erfahren Sie, wie Sie Android-Geräte in Microsoft Intune registrieren.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="36f27-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
