---
title: Fehler beim Überprüfen des Zugriffstokenfehlers beim Einsteigen in Desktop Analytics
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813687"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="1aab8-102">Fehler "Fehler beim Überprüfen des Zugriffstokens" beim Desktop Analytics-Onboarding</span><span class="sxs-lookup"><span data-stu-id="1aab8-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="1aab8-103">Dieser Fehler wird normalerweise beim Ablauf des Authentifizierungstokens beobachtet.</span><span class="sxs-lookup"><span data-stu-id="1aab8-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="1aab8-104">In der Regel aktualisiert das Aktualisieren der Seite das Token.</span><span class="sxs-lookup"><span data-stu-id="1aab8-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="1aab8-105">Dieses Problem kann jedoch bestehen bleiben, wenn Richtlinien für bedingten Zugriff auf das Konto angewendet werden, das für die on-board-Desktopanalyse verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="1aab8-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="1aab8-106">Sie können die Azure AD-Anmeldeprotokolle im Azure-Portal überprüfen, um zu sehen, ob für das Konto, das für das Desktop Analytics-Onboarding verwendet wird, Anmeldefehler gibt.</span><span class="sxs-lookup"><span data-stu-id="1aab8-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="1aab8-107">Weitere Informationen zum bedingten Zugriff finden Sie unter [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="1aab8-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>