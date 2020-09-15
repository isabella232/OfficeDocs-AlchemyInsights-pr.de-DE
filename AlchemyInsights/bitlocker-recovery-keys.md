---
title: BitLocker-Wiederherstellungsschlüssel
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
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685885"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="43d7f-102">Zugreifen auf BitLocker-Wiederherstellungsschlüssel</span><span class="sxs-lookup"><span data-stu-id="43d7f-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="43d7f-103">Wenn Sie BitLocker-Einstellungen für InTune-Endpunktschutz Richtlinien konfigurieren, können Sie festlegen, ob BitLocker-Wiederherstellungsinformationen in Azure Active Directory gespeichert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="43d7f-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="43d7f-104">Wenn diese Einstellung konfiguriert ist, sollten die gespeicherten Wiederherstellungsdaten auf zwei Arten für einen InTune-Administrator als Teil der Gerätedatensatz Daten auf dem Blade "InTune-Geräte" sichtbar sein:</span><span class="sxs-lookup"><span data-stu-id="43d7f-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="43d7f-105">Geräte – Azure AD Geräte – > "Gerät" oder Geräte – > alle Geräte – > "Gerät" – > Wiederherstellungsschlüssel</span><span class="sxs-lookup"><span data-stu-id="43d7f-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="43d7f-106">Alternativ können Sie den Wiederherstellungsschlüssel (Password) sehen, indem Sie den folgenden Befehl an einer Eingabeaufforderung mit erhöhten Rechten ausführen, wenn ein Administratorzugriff auf das Gerät selbst vorliegt:</span><span class="sxs-lookup"><span data-stu-id="43d7f-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="43d7f-107">Wenn das Gerät vor der Registrierung in InTune verschlüsselt wurde, ist der Wiederherstellungsschlüssel möglicherweise dem "Microsoft-Konto" (MSA) zugeordnet, das zum Anmelden beim Gerät während des OOBE-Prozesses verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="43d7f-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="43d7f-108">Wenn dies der Fall ist, sollten beim Zugriff auf  https://onedrive.live.com/recoverykey und bei der Anmeldung mit dieser MSA die Geräte angezeigt werden, für die Wiederherstellungsschlüssel gespeichert wurden.</span><span class="sxs-lookup"><span data-stu-id="43d7f-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="43d7f-109">Wenn das Gerät aufgrund der Konfiguration über eine domänenbasierte Gruppenrichtlinie verschlüsselt wurde, werden die Wiederherstellungsinformationen möglicherweise in der lokalen Active Directory gespeichert.</span><span class="sxs-lookup"><span data-stu-id="43d7f-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

