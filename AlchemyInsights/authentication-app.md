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
# <a name="authentication-app"></a><span data-ttu-id="632b2-102">Authentifizierungs-App</span><span class="sxs-lookup"><span data-stu-id="632b2-102">Authentication app</span></span>

<span data-ttu-id="632b2-103">Wenn Sie ein globaler Administrator sind, können Sie mithilfe der Anmeldediagnose schnell herausfinden, was passiert ist, oder Probleme im Zusammenhang mit der Benutzer anmeldung [diagnostizieren.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="632b2-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="632b2-104">Starten Sie die Diagnose, indem Sie auf die Schaltfläche Diagnose[starten](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)klicken.</span><span class="sxs-lookup"><span data-stu-id="632b2-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="632b2-105">Suchen Sie nach dem zu analysierenden Ereignis, indem Sie die Details zu Benutzer, Anwendung, Anmeldezeit, Anforderungs-ID oder Korrelations-ID eingeben.</span><span class="sxs-lookup"><span data-stu-id="632b2-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="632b2-106">Überprüfen Sie die Diagnoseergebnisse mit den Details des Vorfalls und den Maßnahmen, die Sie ergreifen können, um Änderungen vorzunehmen, falls Änderungen erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="632b2-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="632b2-107">**Überprüfen Sie das zutreffende Szenario:**</span><span class="sxs-lookup"><span data-stu-id="632b2-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="632b2-108">Wenn ein Benutzer keine Pushbenachrichtigung in der Microsoft Authenticator-App bekommt, stellen Sie sicher, dass er nicht unter den blockierten MFA-Benutzern angezeigt wird, wie unter Blockieren und Aufheben der Blockierung von [Benutzern beschrieben.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="632b2-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="632b2-109">Wenn der Benutzer nicht für MFA blockiert ist, aber keine Pushbenachrichtigung erhält, kann er die Microsoft Authenticator-App öffnen, die die ausstehenden Genehmigungsanforderungen zurückziehen wird.</span><span class="sxs-lookup"><span data-stu-id="632b2-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="632b2-110">Als alternative Anmeldemethode kann der Benutzer auch auf Andere Weise auf Signieren klicken und einen Überprüfungscode aus meiner mobilen App verwenden auswählen.</span><span class="sxs-lookup"><span data-stu-id="632b2-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="632b2-111">Die Microsoft Authenticator App ist die einzige verfügbare Methode für viele Benutzer.</span><span class="sxs-lookup"><span data-stu-id="632b2-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="632b2-112">[Weitere Informationen zu Sicherheitseinstellungen](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)finden Sie unter [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) für häufig gestellte Fragen und deren Lösung.</span><span class="sxs-lookup"><span data-stu-id="632b2-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="632b2-113">**Empfohlene Videos**</span><span class="sxs-lookup"><span data-stu-id="632b2-113">**Recommended Videos**</span></span>

<span data-ttu-id="632b2-114">[Einrichten der Authenticator App auf einem neuen Telefon (2Min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="632b2-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
