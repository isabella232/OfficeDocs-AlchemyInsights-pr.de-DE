---
title: Probleme mit dem bedingten Zugriff
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013951"
---
# <a name="conditional-access-issues"></a>Probleme mit dem bedingten Zugriff

**Beheben von Problemen mit der Anmeldediagnose**

Sie können schnell herausfinden, was passiert ist, oder Probleme im Zusammenhang mit der Benutzer anmeldung mithilfe der [Anmeldediagnose diagnostizieren:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Starten Sie die Anmeldediagnose.
1. Suchen Sie das zu analysierende Ereignis, indem Sie die Details zu Benutzer, Anwendung, Zeitpunkt der Anmeldung, Anforderungs-ID oder Korrelations-ID eingeben.
1. Überprüfen Sie die Diagnoseergebnisse, in denen die Details zu den Vorfall und die Aktionen angezeigt werden, die Sie ergreifen können, um Änderungen vorzunehmen (falls Änderungen erforderlich sind).

**Schritte zur Problembehandlung bei einer Anmeldung** 

1. Navigieren Sie zur Azure AD-Anmeldeseite.
1. Filtern Sie Anmeldungen nach Benutzer, Zeitraum, Anwendung, Status, Client-App und so weiter.
1. Wählen Sie ein Anmeldeereignis aus, und zeigen Sie die Registerkarte "Bedingter Zugriff" an, um zu sehen, welche Richtlinien ausgewertet wurden.
1. Klicken Sie auf die Zeile einer Richtlinie, um die Richtliniendetails anzuzeigen und zu verstehen, warum sie angewendet wurde.

**Tools zur Problembehandlung für eine Richtlinie für bedingten Zugriff**

- Im Nur-Berichts-Modus können Sie eine Richtlinie auswerten, ohne sich auf die Benutzer auszu auswirken.
- Mit dem Tool "Was-wäre-wenn" können Sie Anmeldeereignisse simulieren und sehen, welche Richtlinien gelten.
- Die Arbeitsmappe "Einblicke und Berichterstellung" zeigt die Auswirkungen jeder Richtlinie in Echtzeit an.

**Grundlegende Schutzrichtlinien**

Baseline Protection policies have been deprecated. Sie werden nicht mehr erzwungen und werden bald aus dem Azure-Portal entfernt. Es wird empfohlen, [Die Sicherheitseinstellungen zu aktivieren.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

Weitere Informationen zum bedingten Zugriff finden Sie unter:

[Bewährte Methoden für bedingten Zugriff in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Bedingungen im bedingten Zugriff](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Steuerelemente im bedingten Zugriff](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Speicherorte im bedingten Zugriff](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
