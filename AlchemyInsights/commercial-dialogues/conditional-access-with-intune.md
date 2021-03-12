---
title: Verwenden des bedingten Zugriffs mit Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736768"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="8f5e9-102">Verwenden des bedingten Zugriffs mit Intune</span><span class="sxs-lookup"><span data-stu-id="8f5e9-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="8f5e9-103">Für die Verwendung des bedingten Zugriffs mit Intune sind drei Schritte erforderlich:</span><span class="sxs-lookup"><span data-stu-id="8f5e9-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="8f5e9-104">Erstellen Sie eine Compliancerichtlinie, um Einstellungen zu definieren, die erfüllt sein müssen, bevor das Gerät als kompatibel betrachtet wird. Beispielsweise muss ein Gerät eine Pin von mindestens 6 Ziffern haben, bevor es als kompatibel betrachtet wird.</span><span class="sxs-lookup"><span data-stu-id="8f5e9-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="8f5e9-105">Erstellen Sie eine Richtlinie für bedingten Zugriff, die definiert, welche Ressourcen geschützt werden und welche Bedingungen für den Zugriff auf diese Ressourcen erfüllt sein müssen. Beispielsweise muss ein Gerät vor dem Zugriff auf Unternehmens-E-Mails kompatibel sein.</span><span class="sxs-lookup"><span data-stu-id="8f5e9-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="8f5e9-106">Stellen Sie sicher, dass sowohl Compliancerichtlinien als auch Richtlinien für bedingten Zugriff auf die gewünschten Benutzergruppen ausgerichtet sind. Dies kann das Erstellen bestimmter Benutzergruppen in Azure Active Directory erfordern.</span><span class="sxs-lookup"><span data-stu-id="8f5e9-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="8f5e9-107">Weitere Informationen...</span><span class="sxs-lookup"><span data-stu-id="8f5e9-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
