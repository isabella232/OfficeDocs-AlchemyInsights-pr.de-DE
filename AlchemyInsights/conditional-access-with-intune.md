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
# <a name="conditional-access-with-intune"></a>Bedingter Zugriff mit Intune

Für  **die Verwendung des bedingten**  Zugriffs mit Intune sind drei Schritte erforderlich:

- Erstellen Sie  **eine Compliancerichtlinie**  ([Android,](https://docs.microsoft.com/intune/compliance-policy-create-android)  [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios)  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), um Einstellungen zu definieren, die erfüllt sein müssen, bevor das Gerät als kompatibel betrachtet wird. Beispielsweise muss ein Gerät eine Pin von mindestens 6 Ziffern haben, bevor es als kompatibel betrachtet wird.
- Erstellen Sie **eine Richtlinie für bedingten**  Zugriff, die definiert, welche Ressourcen geschützt werden und welche Bedingungen für den Zugriff auf diese Ressourcen erfüllt sein müssen.  [Beispielsweise muss ein](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  Gerät vor dem Zugriff auf Unternehmens-E-Mails kompatibel sein.
- Stellen Sie **sicher, dass sowohl Compliancerichtlinien**  als  **auch Richtlinien für**  bedingten Zugriff auf die gewünschten Benutzergruppen ausgerichtet sind. Dies kann das Erstellen bestimmter Benutzergruppen in Azure Active Directory erfordern.

**Hilfreiche Links:**

[Übersicht über die Gerätekonformität](https://docs.microsoft.com/intune/device-compliance-get-started)

[Problembehandlung bei der Zertifizierungsstelle](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Problembehandlungsrichtlinie](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Um E-Mail (Exchange online) vor dem Zugriff durch nicht kompatible Geräte zu schützen, müssen beide Dokumente befolgt werden:

1. [Schützen des E-Mail-Zugriffs von Geräten mithilfe von EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Schützen des E-Mail-Zugriffs von Geräten mithilfe moderner Authentifizierungsclients wie Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)