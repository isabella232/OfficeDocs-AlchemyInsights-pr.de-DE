---
title: Active Directory nicht synchronisiert
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265195"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="4fbde-102">Active Directory nicht synchronisiert</span><span class="sxs-lookup"><span data-stu-id="4fbde-102">Active Directory not syncing</span></span>

<span data-ttu-id="4fbde-103">Wenn Sie Synchronisierungsfehler wie "keine neuere Synchronisierung" oder den Status "Verzeichnissynchronisierung" im Office-Verwaltungsportal erhalten, sagt "Zuletzt synchronisiert vor mehr als 3 Tagen", kann es sein, dass AADConnect falsche Einstellungen oder unzureichende Berechtigungen zum Durchführen einer Synchronisierung.</span><span class="sxs-lookup"><span data-stu-id="4fbde-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="4fbde-104">Durch die Neuinstallation von AADConnect mithilfe von Express-Einstellungen kann das Problem schnell behoben werden:</span><span class="sxs-lookup"><span data-stu-id="4fbde-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="4fbde-105">[Laden Sie die neueste Version von AADConnect herunter](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="4fbde-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="4fbde-106">[Befolgen Sie die Anweisungen für die Express Installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="4fbde-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="4fbde-107">Weitere Informationen zu AADConnect-Dienstkonten finden Sie unter [Azure AD Connect: Accounts and Permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="4fbde-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
