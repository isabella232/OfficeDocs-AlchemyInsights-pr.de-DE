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
# <a name="conditional-access-with-intune"></a>Bedingter Zugriff mit InTune

Die Verwendung von **bedingtem Zugriff** mit InTune erfordert 3 Schritte:

- Erstellen Sie eine **Konformitätsrichtlinie** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [IOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)), um Einstellungen zu definieren, die erfüllt sein müssen, bevor das Gerät als konform betrachtet wird. Ein Gerät muss beispielsweise eine PIN von mindestens 6 Ziffern aufweisen, bevor es als konform gilt.
- Erstellen Sie eine **Richtlinie für den bedingten Zugriff** , die definiert, welche Ressourcen geschützt werden, und welche Bedingungen erfüllt sein müssen, um auf diese Ressourcen zuzugreifen.  Beispielsweise muss ein Gerät kompatibel sein [,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) bevor auf Firmen-e-Mails zugegriffen werden kann.
- Stellen Sie sicher, dass sowohl **Konformitätsrichtlinien** als auch **Richtlinien für bedingten Zugriff** auf die gewünschten Benutzergruppen zugeschnitten sind. Dies erfordert möglicherweise das Erstellen bestimmter Benutzergruppen in Azure Active Directory.

**Hilfreiche Links:**

[Übersicht über die Gerätekompatibilität](https://docs.microsoft.com/intune/device-compliance-get-started)

[Problembehandlung bei ca](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Problem behandlungsrichtlinie](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Um e-Mails (Exchange Online) vor Zugriff durch nicht konforme Geräte zu schützen, müssen beide Dokumente befolgt werden:

1. [Schützen des e-Mail-Zugriffs von Geräten mit EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Schützen des e-Mail-Zugriffs von Geräten mit modernen Authentifizierungsclients wie Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)