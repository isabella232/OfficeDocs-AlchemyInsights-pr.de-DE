---
title: Bedingter Zugriff mit InTune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931429"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="83281-102">Bedingter Zugriff mit InTune</span><span class="sxs-lookup"><span data-stu-id="83281-102">Conditional Access with Intune</span></span>

<span data-ttu-id="83281-103">Die Verwendung von **bedingtem Zugriff** mit InTune erfordert 3 Schritte:</span><span class="sxs-lookup"><span data-stu-id="83281-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="83281-104">Erstellen Sie eine **Konformitätsrichtlinie** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [IOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), um Einstellungen zu definieren, die erfüllt sein müssen, bevor das Gerät als konform betrachtet wird.</span><span class="sxs-lookup"><span data-stu-id="83281-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="83281-105">Ein Gerät muss beispielsweise eine PIN von mindestens 6 Ziffern aufweisen, bevor es als konform gilt.</span><span class="sxs-lookup"><span data-stu-id="83281-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="83281-106">Erstellen Sie eine **Richtlinie für den bedingten Zugriff** , die definiert, welche Ressourcen geschützt werden, und welche Bedingungen erfüllt sein müssen, um auf diese Ressourcen zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="83281-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="83281-107">Beispielsweise muss ein Gerät kompatibel sein [,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) bevor auf Firmen-e-Mails zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="83281-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="83281-108">Stellen Sie sicher, dass sowohl **Konformitätsrichtlinien** als auch **Richtlinien für bedingten Zugriff** auf die gewünschten Benutzergruppen zugeschnitten sind.</span><span class="sxs-lookup"><span data-stu-id="83281-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="83281-109">Dies erfordert möglicherweise das Erstellen bestimmter Benutzergruppen in Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="83281-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="83281-110">**Hilfreiche Links:**</span><span class="sxs-lookup"><span data-stu-id="83281-110">**Helpful links:**</span></span>

[<span data-ttu-id="83281-111">Übersicht über die Gerätekompatibilität</span><span class="sxs-lookup"><span data-stu-id="83281-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="83281-112">Problembehandlung bei ca</span><span class="sxs-lookup"><span data-stu-id="83281-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="83281-113">Problem behandlungsrichtlinie</span><span class="sxs-lookup"><span data-stu-id="83281-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="83281-114">Um e-Mails (Exchange Online) vor Zugriff durch nicht konforme Geräte zu schützen, müssen beide Dokumente befolgt werden:</span><span class="sxs-lookup"><span data-stu-id="83281-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="83281-115">Schützen des e-Mail-Zugriffs von Geräten mit EAS</span><span class="sxs-lookup"><span data-stu-id="83281-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="83281-116">Schützen des e-Mail-Zugriffs von Geräten mit modernen Authentifizierungsclients wie Outlook</span><span class="sxs-lookup"><span data-stu-id="83281-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)