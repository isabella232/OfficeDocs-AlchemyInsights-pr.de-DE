---
title: Geheime Client- oder Zertifikatprobleme bei der App-Registrierung
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123116"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="56182-102">Geheime Client- oder Zertifikatprobleme bei der App-Registrierung</span><span class="sxs-lookup"><span data-stu-id="56182-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="56182-103">Ablauf des Geheimen Anwendungsclients?</span><span class="sxs-lookup"><span data-stu-id="56182-103">Application client secret expiring?</span></span>

<span data-ttu-id="56182-104">Unabhängig davon, wie die registrierte Anwendung erstellt wurde, sei es über den Standardregistrierungsprozess im Apps-Registrierungsportal oder wenn der Dienstprinzipal in Ihrem Mandanten mithilfe der Anwendungs zustimmung erstellt wurde, muss ein neuer Geheimer Clientgeheimnis vor dem Ablauf des aktuellen erstellt und im zugehörigen Anwendungscode aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="56182-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="56182-105">Die maximale Gültigkeitsdauer beträgt 2 Jahre.</span><span class="sxs-lookup"><span data-stu-id="56182-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="56182-106">Zur Erinnerung: Der geheime Wert muss aufgezeichnet werden, da er nach dem Verlassen der Seite "App-Registrierungen" im Portal nicht mehr sichtbar ist.</span><span class="sxs-lookup"><span data-stu-id="56182-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="56182-107">Weitere Informationen finden Sie unter [Schnellstart: Registrieren einer App in](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) der Microsoft Identity Platform und Bewährte Methoden für die Microsoft Identity [Platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span><span class="sxs-lookup"><span data-stu-id="56182-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="56182-108">Weitere Informationen finden Sie unter [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span><span class="sxs-lookup"><span data-stu-id="56182-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
