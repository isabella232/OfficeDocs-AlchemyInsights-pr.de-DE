---
title: Authentifizierungs-App
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403802"
---
# <a name="authentication-app"></a>Authentifizierungs-App

Wenn Sie ein globaler Administrator sind, können Sie mithilfe der Anmeldediagnose schnell herausfinden, was passiert ist, oder Probleme im Zusammenhang mit der Benutzer anmeldung [diagnostizieren.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Starten Sie die Diagnose, indem Sie auf die Schaltfläche Diagnose[starten](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)klicken. 
1. Suchen Sie nach dem zu analysierenden Ereignis, indem Sie die Details zu Benutzer, Anwendung, Anmeldezeit, Anforderungs-ID oder Korrelations-ID eingeben.
1. Überprüfen Sie die Diagnoseergebnisse mit den Details des Vorfalls und den Maßnahmen, die Sie ergreifen können, um Änderungen vorzunehmen, falls Änderungen erforderlich sind.

**Überprüfen Sie das zutreffende Szenario:**

1. Wenn ein Benutzer keine Pushbenachrichtigung in der Microsoft Authenticator-App bekommt, stellen Sie sicher, dass er nicht unter den blockierten MFA-Benutzern angezeigt wird, wie unter Blockieren und Aufheben der Blockierung von [Benutzern beschrieben.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Wenn der Benutzer nicht für MFA blockiert ist, aber keine Pushbenachrichtigung erhält, kann er die Microsoft Authenticator-App öffnen, die die ausstehenden Genehmigungsanforderungen zurückziehen wird.
1. Als alternative Anmeldemethode kann der Benutzer auch auf Andere Weise auf Signieren klicken und einen Überprüfungscode aus meiner mobilen App verwenden auswählen.
1. Die Microsoft Authenticator App ist die einzige verfügbare Methode für viele Benutzer. [Weitere Informationen zu Sicherheitseinstellungen](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)finden Sie unter [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) für häufig gestellte Fragen und deren Lösung.
 
**Empfohlene Videos**

[Einrichten der Authenticator App auf einem neuen Telefon (2Min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
