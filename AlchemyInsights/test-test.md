---
title: Begriffe, die in SharePoint Online Term Store fehlen
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053512"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="13ce6-102">Aktivieren der BitLocker-Verschlüsselung mit InTune</span><span class="sxs-lookup"><span data-stu-id="13ce6-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="13ce6-103">Die Intune-Endpunktschutz Richtlinie kann zum Konfigurieren von Boitlocker-Verschlüsselungseinstellungen für Windows-Geräte verwendet werden, wie unter: Windows10 (und höher) Einstellungen zum Schützen von Geräten mithilfe von InTune beschrieben.</span><span class="sxs-lookup"><span data-stu-id="13ce6-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="13ce6-104">Beachten Sie, dass viele neuere Geräte mit Windows 10 die automatische BitLocker-Verschlüsselung unterstützen, die ohne Anwendung der MDM-Richtlinie ausgelöst wird.</span><span class="sxs-lookup"><span data-stu-id="13ce6-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="13ce6-105">Dies kann sich auf die Anwendung von Richtlinien auswirken, wenn nicht Standardeinstellungen konfiguriert sind.</span><span class="sxs-lookup"><span data-stu-id="13ce6-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="13ce6-106">Weitere Informationen finden Sie unter FAQ.</span><span class="sxs-lookup"><span data-stu-id="13ce6-106">See FAQ for more detail.</span></span>


<span data-ttu-id="13ce6-107">FAQ  f: welche Editionen von Windows unterstützen die Geräteverschlüsselung mithilfe der Endpunktschutz Richtlinie?</span><span class="sxs-lookup"><span data-stu-id="13ce6-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="13ce6-108"> A.: die Einstellungen in der InTune-Endpunktschutz Richtlinie werden mithilfe des BitLocker-CSP implementiert.</span><span class="sxs-lookup"><span data-stu-id="13ce6-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="13ce6-109">Nicht alle Editionen oder Builds von Windows unterstützen den BitLocker-CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="13ce6-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="13ce6-110">Zu diesem Zeitpunkt Windows-Editionen: Enterprise; Education, Mobile, Mobile Enterprise und Professional (ab Build 1809) werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="13ce6-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="13ce6-111">F.: Wenn ein Gerät bereits mit BitLocker mit den Standardeinstellungen für Verschlüsselungsmethode und Verschlüsselungsstärke (XTS-AES-128) verschlüsselt ist, wird eine Richtlinie mit unterschiedlichen Einstellungen automatisch mit der erneuten Verschlüsselung des Laufwerks mit den neuen Einstellungen ausgelöst?</span><span class="sxs-lookup"><span data-stu-id="13ce6-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="13ce6-112">A.: Nein.</span><span class="sxs-lookup"><span data-stu-id="13ce6-112">A: No.</span></span> <span data-ttu-id="13ce6-113">Damit die neuen Verschlüsselungseinstellungen angewendet werden, muss das Laufwerk zunächst entschlüsselt werden.</span><span class="sxs-lookup"><span data-stu-id="13ce6-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="13ce6-114">Hinweis für Geräte, die mit Autopilot registriert werden die automatische Verschlüsselung, die während der OOBE erfolgen würde, wird erst ausgelöst, wenn die Intune-Richtlinie ausgewertet wird, sodass die richtlinienbasierten Einstellungen anstelle der Standardwerte für das Betriebssystem verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="13ce6-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="13ce6-115">F. Wenn ein Gerät aufgrund der Anwendung der InTune-Richtlinie verschlüsselt wird, wird es entschlüsselt, wenn diese Richtlinie entfernt wird?</span><span class="sxs-lookup"><span data-stu-id="13ce6-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="13ce6-116">A: das Entfernen von Verschlüsselungs bezogenen Richtlinien führt nicht zur Entschlüsselung der konfigurierten Laufwerke.</span><span class="sxs-lookup"><span data-stu-id="13ce6-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="13ce6-117">F: Warum zeigt die Intune-Konformitätsrichtlinie an, dass auf meinem Gerät "BitLocker Enabled" nicht vorhanden ist, aber es ist?</span><span class="sxs-lookup"><span data-stu-id="13ce6-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="13ce6-118">A.: die Einstellung "BitLocker Enabled" in der InTune-Konformitätsrichtlinie verwendet den Windows-Client für Geräte Integritäts Bescheinigung (DHA).</span><span class="sxs-lookup"><span data-stu-id="13ce6-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="13ce6-119">Dieser Client misst nur den Gerätestatus zum Zeitpunkt des Bootens.</span><span class="sxs-lookup"><span data-stu-id="13ce6-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="13ce6-120">Wenn also ein Gerät seit der BitLocker-Verschlüsselung nicht neu gestartet wird, meldet der DHA-Client Dienst BitLocker nicht als aktiv.</span><span class="sxs-lookup"><span data-stu-id="13ce6-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>