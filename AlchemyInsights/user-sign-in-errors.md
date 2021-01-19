---
title: Fehler bei der Benutzeranmeldung
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886829"
---
# <a name="user-sign-in-errors"></a><span data-ttu-id="64b78-102">Fehler bei der Benutzeranmeldung</span><span class="sxs-lookup"><span data-stu-id="64b78-102">User sign-in errors</span></span>

<span data-ttu-id="64b78-103">**Beheben von Problemen mit der Anmeldediagnose**</span><span class="sxs-lookup"><span data-stu-id="64b78-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="64b78-104">Führen Sie die folgenden Schritte durch, um die Ursache zu ermitteln oder Probleme im Zusammenhang mit der Benutzeranmeldung zu diagnostizieren:</span><span class="sxs-lookup"><span data-stu-id="64b78-104">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="64b78-105">Starten Sie die [Anmeldediagnose](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="64b78-105">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="64b78-106">Suchen Sie das zu analysierende Ereignis, indem Sie die Details über den Benutzer, die Anwendung, den Zeitpunkt der Anmeldung, die Anfrage-ID oder die Korrelations-ID eingeben.</span><span class="sxs-lookup"><span data-stu-id="64b78-106">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="64b78-107">Überprüfen Sie die Diagnoseergebnisse mit den Details des Vorfalls und den Maßnahmen, die Sie ergreifen können, um Änderungen vorzunehmen, falls Änderungen erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="64b78-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="64b78-108">**Suchen Sie nach Informationen zu den AADSTS-Fehlercodes, die vom Azure Active Directory(Azure AD)-Sicherheitstokendienst (STS) zurückgegeben werden?**</span><span class="sxs-lookup"><span data-stu-id="64b78-108">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="64b78-109">In [diesem Artikel](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) finden Sie AADSTS-Fehlerbeschreibungen, Fehlerbehebungen und einige Vorschläge zur Umgehung des Problems</span><span class="sxs-lookup"><span data-stu-id="64b78-109">Read [this article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds</span></span>