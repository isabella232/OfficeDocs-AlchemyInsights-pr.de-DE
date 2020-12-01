---
title: Endpunkt-DLP-Lizenzierungsfehler
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: d17c51177898d62c7c477460c8c26b4753bae65f
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/30/2020
ms.locfileid: "49477671"
---
# <a name="endpoint-dlp-licensing-error"></a>Endpunkt-DLP-Lizenzierungsfehler

Wenn Sie versuchen, Endpunkt-DLP einzurichten, wenn folgende Fehlermeldung angezeigt wird:

`Your organization is missing the licenses required to manage these devices`.

Stellen Sie sicher, dass Sie über eines der folgenden Abonnements oder Add-ons verfügen:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5 Compliance
- Microsoft 365 A5 Compliance
- Microsoft 365 E5 Information Protection und Governance
- Microsoft 365 A5 Information Protection und Governance

> [!NOTE]
> Dies funktioniert nicht für Lizenz Kombinationen wie: Win E5 + O365 E5 + EMS E5. Zum Einrichten dieses Features benötigen Sie eine reine M365 E5-Lizenz.

Weitere Informationen zur Endpunkt-DLP-Lizenzierung finden Sie unter [EndPoint DLP Licensing.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
