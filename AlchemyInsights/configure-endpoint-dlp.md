---
title: Konfigurieren von Endpunkt-DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402421"
---
# <a name="configure-endpoint-dlp"></a>Konfigurieren von Endpunkt-DLP

Microsoft Endpunkt-DLP bietet Ihnen die Möglichkeit, Schutz- und Überwachungsfunktionen von DLP auf vertrauliche Informationen auf Windows 10-Geräten zu erweitern. Nachdem die Geräte in die Geräteverwaltung integriert wurden, können Sie DLP-Richtlinien erstellen, um Schutzmaßnahmen für Objekte durchzusetzen. Der Aktivitäten-Explorer kann verwendet werden, um die Aktivität für vertrauliche Elemente zu überwachen. Weitere Informationen finden Sie unter [Onboarding von Geräten für die Geräteverwaltung](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

So führen Sie die ersten Schritte mit Endpunkt-DLP aus

- Stellen Sie sicher, dass Sie über die geeignete SKU/Abonnementlizenzierung verfügen. Weitere Informationen finden Sie unter [SKU/Abonnement-Lizenzierung](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Überprüfen Sie die Berechtigungen, die erforderlich sind, um die Geräteverwaltung zu aktivieren, auf die Onboardingseite zuzugreifen oder die Geräteüberwachung ein- und auszuschalten. Weitere Informationen finden Sie unter [Berechtigungen](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Führen Sie ein Onboarding der Geräte in die Geräteverwaltung aus, indem Sie dem Verfahren für das Onboarding von Geräten folgen. Wenn Sie die Option "Geräte-Onboarding (Vorschau)" unter M365 Compliance > **Einstellungen** vermissen, überprüfen Sie, ob Sie über die entsprechende Lizenz und die entsprechenden Berechtigungen verfügen, auf die oben verwiesen wird. Weitere Informationen finden Sie unter [Onboarding von Geräten](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Erstellen Sie DLP-Richtlinien zum Schutz Ihrer vertraulichen Elemente. Informationen hierzu finden Sie unter [Szenarien für Endpunkt-DLP-Richtlinien](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

Weitere Informationen zu Microsoft Endpunkt-DLP finden Sie unter [Informationen zu Microsoft 365 Endpunkt-DLP (Data Loss Prevention, Verhinderung von Datenverlust) (Vorschau)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Wichtige Datenerfassungsschritte, falls Support benötigt wird:**

1. MDATP Client Analyzer-Vorschauversion von [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer") herunterladen
2. Führen Sie das Tool über das CMD-Fenster als Administrator aus:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. Wenn Sie mit "Geben Sie die Anzahl der Minuten ein, in denen die Ablaufverfolgungen erfasst werden soll" aufgefordert werden, geben Sie Dauer, die für die Ausführung des Szenarios erforderlich ist, in Minuten ein.
5. Ausführen des Szenarios

Erfassen Sie die ZIP-Dateiausgabe, um sie dem Supportmitarbeiter zu übergeben.
