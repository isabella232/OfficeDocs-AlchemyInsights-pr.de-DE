---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768816"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="84c70-102">Aktivieren der BitLocker-Verschlüsselung mit InTune</span><span class="sxs-lookup"><span data-stu-id="84c70-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="84c70-103">Die Intune-Endpunktschutz Richtlinie kann zum Konfigurieren von BitLocker-Verschlüsselungseinstellungen für Windows-Geräte verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="84c70-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="84c70-104">Weitere Informationen finden Sie unter [Einstellungen für Windows 10 (und höher), um Geräte mit InTune zu schützen](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="84c70-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="84c70-105">Beachten Sie, dass viele neuere Geräte mit Windows 10 die automatische BitLocker-Verschlüsselung unterstützen, die ohne Anwendung der MDM-Richtlinie ausgelöst wird.</span><span class="sxs-lookup"><span data-stu-id="84c70-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="84c70-106">Dies kann sich auf die Anwendung von Richtlinien auswirken, wenn nicht standardmäßige Einstellungen konfiguriert werden.</span><span class="sxs-lookup"><span data-stu-id="84c70-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="84c70-107">Weitere Informationen finden Sie in den folgenden FAQ.</span><span class="sxs-lookup"><span data-stu-id="84c70-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="84c70-108">Informationen zur Behandlung von BitLocker-Problemen finden Sie unter [Problembehandlung für BitLocker-Richtlinien in Microsoft InTune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="84c70-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="84c70-109">**Häufig gestellte Fragen**</span><span class="sxs-lookup"><span data-stu-id="84c70-109">**FAQ**</span></span>

<span data-ttu-id="84c70-110">F.: welche Editionen von Windows unterstützen die Geräteverschlüsselung mithilfe der Endpunktschutz Richtlinie?</span><span class="sxs-lookup"><span data-stu-id="84c70-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="84c70-111">A.: die Einstellungen in der InTune-Endpunktschutz Richtlinie werden mithilfe des [BitLocker-CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)implementiert.</span><span class="sxs-lookup"><span data-stu-id="84c70-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="84c70-112">Nicht alle Editionen oder Builds von Windows unterstützen den BitLocker-CSP.</span><span class="sxs-lookup"><span data-stu-id="84c70-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="84c70-113">F: Wie kann BitLocker auf Geräten aktiviert werden, ohne dass eine Benutzerinteraktion erforderlich ist?</span><span class="sxs-lookup"><span data-stu-id="84c70-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="84c70-114">A: solange die erforderlichen Voraussetzungen erfüllt sind, kann BitLocker "Silent Encryption" über InTune aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="84c70-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="84c70-115">Lesen Sie die Details der Geräteanforderungen und Beispiel Richtlinieneinstellungen zum Aktivieren der automatischen Verschlüsselung im folgenden Dokument: [Automatische BitLocker-Verschlüsselung aktivieren](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span><span class="sxs-lookup"><span data-stu-id="84c70-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="84c70-116">F.: Wenn ein Gerät bereits mit BitLocker mit den Standardeinstellungen für Verschlüsselungsmethode und Verschlüsselungsstärke (XTS-AES-128) verschlüsselt ist, wird durch die Anwendung einer Richtlinie mit unterschiedlichen Einstellungen automatisch eine erneute Verschlüsselung des Laufwerks mit den neuen Einstellungen ausgelöst?</span><span class="sxs-lookup"><span data-stu-id="84c70-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="84c70-117">A: Nein.</span><span class="sxs-lookup"><span data-stu-id="84c70-117">A: No.</span></span> <span data-ttu-id="84c70-118">Damit die neuen Verschlüsselungseinstellungen angewendet werden, muss das Laufwerk zunächst entschlüsselt werden.</span><span class="sxs-lookup"><span data-stu-id="84c70-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="84c70-119">**Hinweis:** Für Geräte, die mit Autopilot registriert werden, wird die automatische Verschlüsselung, die während der OOBE erfolgen würde, erst ausgelöst, wenn die Intune-Richtlinie ausgewertet wird, sodass die richtlinienbasierten Einstellungen anstelle der Standardwerte für das Betriebssystem verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="84c70-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="84c70-120">F.: wird ein Gerät aufgrund der Anwendung der InTune-Richtlinie verschlüsselt, wird es entschlüsselt, wenn diese Richtlinie entfernt wird?</span><span class="sxs-lookup"><span data-stu-id="84c70-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="84c70-121">A: das Entfernen einer Verschlüsselungs bezogenen Richtlinie führt nicht zur Entschlüsselung der konfigurierten Laufwerke.</span><span class="sxs-lookup"><span data-stu-id="84c70-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="84c70-122">F: Warum zeigt die Intune-Konformitätsrichtlinie an, dass für mein Gerät BitLocker nicht aktiviert ist, obwohl dies der Fall ist?</span><span class="sxs-lookup"><span data-stu-id="84c70-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="84c70-123">A.: die Einstellung "BitLocker Enabled" in der InTune-Konformitätsrichtlinie verwendet den Windows-Client für Geräte Integritäts Bescheinigung (DHA).</span><span class="sxs-lookup"><span data-stu-id="84c70-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="84c70-124">Dieser Client misst nur den Gerätestatus zum Zeitpunkt des Bootens.</span><span class="sxs-lookup"><span data-stu-id="84c70-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="84c70-125">Wenn also ein Gerät seit der BitLocker-Verschlüsselung nicht neu gestartet wurde, meldet der DHA-Client Dienst BitLocker nicht als aktiv.</span><span class="sxs-lookup"><span data-stu-id="84c70-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 