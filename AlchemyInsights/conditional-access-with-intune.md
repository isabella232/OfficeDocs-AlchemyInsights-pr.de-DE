---
title: Bedingter Zugriff mit Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704785"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="83d75-102">Bedingter Zugriff mit Intune</span><span class="sxs-lookup"><span data-stu-id="83d75-102">Conditional Access with Intune</span></span>

<span data-ttu-id="83d75-103">Für  **die Verwendung des bedingten**  Zugriffs mit Intune sind drei Schritte erforderlich:</span><span class="sxs-lookup"><span data-stu-id="83d75-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="83d75-104">Erstellen Sie  **eine Compliancerichtlinie**  ([Android,](https://docs.microsoft.com/intune/compliance-policy-create-android)  [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios)  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), um Einstellungen zu definieren, die erfüllt sein müssen, bevor das Gerät als kompatibel betrachtet wird.</span><span class="sxs-lookup"><span data-stu-id="83d75-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="83d75-105">Beispielsweise muss ein Gerät eine Pin von mindestens 6 Ziffern haben, bevor es als kompatibel betrachtet wird.</span><span class="sxs-lookup"><span data-stu-id="83d75-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="83d75-106">Erstellen Sie **eine Richtlinie für bedingten**  Zugriff, die definiert, welche Ressourcen geschützt werden und welche Bedingungen für den Zugriff auf diese Ressourcen erfüllt sein müssen.</span><span class="sxs-lookup"><span data-stu-id="83d75-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="83d75-107">[Beispielsweise muss ein](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  Gerät vor dem Zugriff auf Unternehmens-E-Mails kompatibel sein.</span><span class="sxs-lookup"><span data-stu-id="83d75-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="83d75-108">Stellen Sie **sicher, dass sowohl Compliancerichtlinien**  als  **auch Richtlinien für**  bedingten Zugriff auf die gewünschten Benutzergruppen ausgerichtet sind.</span><span class="sxs-lookup"><span data-stu-id="83d75-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="83d75-109">Dies kann das Erstellen bestimmter Benutzergruppen in Azure Active Directory erfordern.</span><span class="sxs-lookup"><span data-stu-id="83d75-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="83d75-110">**Hilfreiche Links:**</span><span class="sxs-lookup"><span data-stu-id="83d75-110">**Helpful links:**</span></span>

[<span data-ttu-id="83d75-111">Übersicht über die Gerätekonformität</span><span class="sxs-lookup"><span data-stu-id="83d75-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="83d75-112">Problembehandlung bei der Zertifizierungsstelle</span><span class="sxs-lookup"><span data-stu-id="83d75-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="83d75-113">Problembehandlungsrichtlinie</span><span class="sxs-lookup"><span data-stu-id="83d75-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="83d75-114">Um E-Mail (Exchange online) vor dem Zugriff durch nicht kompatible Geräte zu schützen, müssen beide Dokumente befolgt werden:</span><span class="sxs-lookup"><span data-stu-id="83d75-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="83d75-115">Schützen des E-Mail-Zugriffs von Geräten mithilfe von EAS</span><span class="sxs-lookup"><span data-stu-id="83d75-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="83d75-116">Schützen des E-Mail-Zugriffs von Geräten mithilfe moderner Authentifizierungsclients wie Outlook</span><span class="sxs-lookup"><span data-stu-id="83d75-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)