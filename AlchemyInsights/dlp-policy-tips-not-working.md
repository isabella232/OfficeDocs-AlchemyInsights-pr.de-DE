---
title: DLP-Richtlinien Tipps funktionieren nicht
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932585"
---
# <a name="dlp-policy-tip-issues"></a>Probleme mit dem DLP-richtlinientipp

**Wichtig**: viele SharePoint Online-und OneDrive-Kunden führen geschäftskritische Anwendungen für den Dienst aus, der im Hintergrund ausgeführt wird. Dazu gehören Inhaltsmigration, Verhinderung von Datenverlusten (Data Loss Prevention, DLP) und Sicherungslösungen. In diesen noch nie dagewesenen Zeiten machen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online- und OneDrive-Dienste für Ihre Benutzer, die von dem Dienst in Remotearbeitsszenarien mehr denn je abhängig sind, weiterhin hochgradig verfügbar und zuverlässig sind.

Zur Unterstützung dieses Ziels haben wir strengere Drosselungsgrenzen für Hintergrundanwendungen (Migration, DLP und Sicherungslösungen) während der Tageszeit unter der Woche eingeführt. Sie sollten davon ausgehen, dass diese Apps in diesen Zeiten einen sehr begrenzten Durchsatz erreichen. Während der Abendstunden und an Wochenenden wird der Dienst für die Region jedoch in der Lage sein, ein erheblich höheres Volumen an Anforderungen von Hintergrundanwendungen zu verarbeiten.

**DLP-Richtlinien Tipps**

Bei der Verwendung von **DLP-Richtlinien**können Benutzer über eine Richtlinienverletzung mit **Richtlinien Tipps**informiert werden. Administratoren können Richtlinien Tipps so konfigurieren, dass Sie beim Testen Ihrer DLP-Richtlinie angezeigt werden oder wenn sich die Richtlinie im vollständigen Erzwingungsmodus befindet.
  
Gehen Sie folgendermaßen vor, um Richtlinien Tipps für ihre DLP-Richtlinie im Security and Compliance Center im vollständigen Durchsetzungs Modus zu konfigurieren:
  
- Stellen Sie sicher, dass in der DLP-Regel mithilfe der [hier](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)beschriebenen Schritte Richtlinien Tipps **aktiviert** wurden.

- Stellen Sie sicher, dass Ihre Inhalte [hier](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for) **übereinstimmen** , die **erforderlich** sind, um die in diesem Artikel dargelegte Regel auszulösen.

- Richtlinien Tipps werden sowohl in OWA als auch in Outlook angezeigt. Wenn Sie jedoch **Outlook 2013 oder höher**verwenden, werden Richtlinien Tipps nur unter bestimmten Bedingungen angezeigt. Diese Bedingungen sind hier aufgelistet: [unterstützte Bedingungen für Outlook 2013 oder höher zum Anzeigen von Richtlinien Tipps](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)

Weitere Informationen zu DLP-Richtlinien Tipps finden Sie unter: [Anzeigen von Richtlinien Tipps für DLP-Richtlinien](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
  