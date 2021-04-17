---
title: Bitlocker-Wiederherstellungsschlüssel
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820285"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="a985c-102">Zugreifen auf Bitlocker-Wiederherstellungsschlüssel</span><span class="sxs-lookup"><span data-stu-id="a985c-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="a985c-103">Beim Konfigurieren der Intune Endpoint Protection-Richtlinie für Bitlockereinstellungen kann definiert werden, ob Bitlocker-Wiederherstellungsinformationen in Azure Active Directory gespeichert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="a985c-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="a985c-104">Wenn diese Einstellung konfiguriert ist, sollten die gespeicherten Wiederherstellungsdaten für einen Intune-Administrator als Teil der Gerätedaten im Blatt Intune Devices auf zwei Arten sichtbar sein:</span><span class="sxs-lookup"><span data-stu-id="a985c-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="a985c-105">Geräte - Azure AD-Geräte -> "Gerät" ODER Geräte -> Alle Geräte -> "Device" -> Wiederherstellungsschlüssel</span><span class="sxs-lookup"><span data-stu-id="a985c-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="a985c-106">Wenn Administratorzugriff auf das Gerät selbst besteht, kann der Wiederherstellungsschlüssel (Password) durch Ausführen des folgenden Befehls an einer Eingabeaufforderung mit erhöhten Rechten angezeigt werden:</span><span class="sxs-lookup"><span data-stu-id="a985c-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="a985c-107">Wenn das Gerät vor der Registrierung in Intune verschlüsselt wurde, wurde der Wiederherstellungsschlüssel möglicherweise dem "Microsoft Account" (MSA) zugeordnet, mit dem sich das Gerät während des OOBE-Prozesses anmeldete.</span><span class="sxs-lookup"><span data-stu-id="a985c-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="a985c-108">Wenn dies der Fall war, sollten beim Zugriff und der Anmeldung mit dieser MSA die Geräte angezeigt werden, für die Wiederherstellungsschlüssel  https://onedrive.live.com/recoverykey gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="a985c-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="a985c-109">Wenn das Gerät aufgrund der Konfiguration über eine domänenbasierte Gruppenrichtlinie verschlüsselt wurde, können die Wiederherstellungsinformationen im lokalen Active Directory gespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="a985c-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="a985c-110">Wenn Sie die Endpoint Protection-Richtlinie so konfiguriert haben, dass der Wiederherstellungsschlüssel in Azure Active Directory gespeichert wird, der Schlüssel für ein bestimmtes Gerät jedoch nicht hochgeladen wurde, können Sie den Upload auslösen, indem Sie den Wiederherstellungsschlüssel für dieses Gerät aus der MEM-Konsole drehen.</span><span class="sxs-lookup"><span data-stu-id="a985c-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="a985c-111">Weitere Informationen finden Sie unter [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span><span class="sxs-lookup"><span data-stu-id="a985c-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

