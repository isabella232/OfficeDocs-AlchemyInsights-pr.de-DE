---
title: BitLocker-Wiederherstellungsschlüssel
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908814"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="82e76-102">Zugreifen auf BitLocker-Wiederherstellungsschlüssel</span><span class="sxs-lookup"><span data-stu-id="82e76-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="82e76-103">Wenn Sie BitLocker-Einstellungen für InTune-Endpunktschutz Richtlinien konfigurieren, können Sie festlegen, ob BitLocker-Wiederherstellungsinformationen in Azure Active Directory gespeichert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="82e76-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="82e76-104">Wenn diese Einstellung konfiguriert ist, sollten die gespeicherten Wiederherstellungsdaten auf zwei Arten für einen InTune-Administrator als Teil der Gerätedatensatz Daten auf dem Blade "InTune-Geräte" sichtbar sein:</span><span class="sxs-lookup"><span data-stu-id="82e76-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="82e76-105">Geräte – Azure AD Geräte – #a0 "Gerät" oder Geräte – #a1 alle Geräte – #a2 "Gerät" – #a3 Wiederherstellungsschlüssel</span><span class="sxs-lookup"><span data-stu-id="82e76-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="82e76-106">Alternativ können Sie den Wiederherstellungsschlüssel (Password) sehen, indem Sie den folgenden Befehl an einer Eingabeaufforderung mit erhöhten Rechten ausführen, wenn ein Administratorzugriff auf das Gerät selbst vorliegt:</span><span class="sxs-lookup"><span data-stu-id="82e76-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
<span data-ttu-id="82e76-107">Wenn das Gerät vor der Registrierung in InTune verschlüsselt wurde, ist der Wiederherstellungsschlüssel möglicherweise dem "Microsoft-Konto" (MSA) zugeordnet, das zum Anmelden beim Gerät während des OOBE-Prozesses verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="82e76-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="82e76-108">Wenn dies der Fall ist, sollten https://onedrive.live.com/recoverykey beim Zugriff auf und bei der Anmeldung mit dieser MSA die Geräte angezeigt werden, für die Wiederherstellungsschlüssel gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="82e76-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="82e76-109">Wenn das Gerät aufgrund der Konfiguration über eine domänenbasierte Gruppenrichtlinie verschlüsselt wurde, werden die Wiederherstellungsinformationen möglicherweise in der lokalen Active Directory gespeichert.</span><span class="sxs-lookup"><span data-stu-id="82e76-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

