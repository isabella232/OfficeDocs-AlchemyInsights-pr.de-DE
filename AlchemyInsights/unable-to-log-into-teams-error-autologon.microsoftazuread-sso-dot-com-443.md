---
title: Die Anmeldung bei Teams ist aufgrund des Fehlers „autologon.microsoftazuread-sso.com:443“ nicht möglich.
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931899"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="bd640-102">Die Anmeldung bei Teams ist aufgrund des Fehlers „autologon.microsoftazuread-sso dot com:443“ nicht möglich.</span><span class="sxs-lookup"><span data-stu-id="bd640-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="bd640-103">Wenn das nahtlose einmalige Anmelden als O365-Authentifizierung aktiviert ist, muss die URL "autologon.microsoftazuread-sso.com" möglicherweise zu den Intranetsites hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="bd640-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="bd640-104">Wenn es zuvor zu vertrauenswürdigen Websites hinzugefügt wurde und nahtloses einmaliges Anmelden verwendet wird, sollte es aus den vertrauenswürdigen Websites entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="bd640-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="bd640-105">Sehen Sie sich die Checkliste unter [Problembehandlung beim nahtlosen einmaligen Anmelden](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist) an.</span><span class="sxs-lookup"><span data-stu-id="bd640-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="bd640-106">Befolgen Sie diese Schritte, um eine URL zur Liste der Intranetsites hinzuzufügen:</span><span class="sxs-lookup"><span data-stu-id="bd640-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="bd640-107">Öffnen Sie Internet Explorer, indem Sie auf die Schaltfläche**Start** klicken.</span><span class="sxs-lookup"><span data-stu-id="bd640-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="bd640-108">Geben Sie im Suchfeld „Internet Explorer“ ein, und klicken Sie dann in der Liste der Ergebnisse auf **Internet Explorer**.</span><span class="sxs-lookup"><span data-stu-id="bd640-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="bd640-109">Klicken Sie auf **Extras**, und klicken Sie anschließend auf **Internetoptionen**.</span><span class="sxs-lookup"><span data-stu-id="bd640-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="bd640-110">Klicken Sie auf die Registerkarte **Sicherheit**.</span><span class="sxs-lookup"><span data-stu-id="bd640-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="bd640-111">Klicken Sie nun auf **Lokales Intranet** und dann auf die Schaltfläche **Sites** und auf **Erweitert**.</span><span class="sxs-lookup"><span data-stu-id="bd640-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="bd640-112">Geben Sie die Website-URL ein, und klicken Sie auf **Hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="bd640-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="bd640-113">Klicken Sie nach Abschluss des Vorgangs auf **Schließen**.</span><span class="sxs-lookup"><span data-stu-id="bd640-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="bd640-114">Weitere Informationen finden Sie unter [Dokumentation zur Bereitstellung von nahtlosem einmaligen Anmelden für O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (enthält den richtlinienbasierten Prozess zum Hinzufügen einer URL zu den Intranetsites in Schritt 3).</span><span class="sxs-lookup"><span data-stu-id="bd640-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
