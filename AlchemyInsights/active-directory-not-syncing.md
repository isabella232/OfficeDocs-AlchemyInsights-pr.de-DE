---
title: Active Directory wird nicht synchronisiert
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
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930974"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="1f60c-102">Active Directory wird nicht synchronisiert</span><span class="sxs-lookup"><span data-stu-id="1f60c-102">Active Directory not syncing</span></span>

<span data-ttu-id="1f60c-103">Wenn Sie Synchronisierungsfehler erhalten, z. B. "keine aktuelle Synchronisierung", oder beachten Sie, dass der Status der Verzeichnissynchronisierung im Office Verwaltungsportal besagt: "Letzte Synchronisierung vor mehr als 3 Tagen", kann es sein, dass AADConnect über falsche Einstellungen oder unzureichende Berechtigungen zum Ausführen einer Synchronisierung verfügt.</span><span class="sxs-lookup"><span data-stu-id="1f60c-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="1f60c-104">Durch erneutes Installieren von AADConnect mithilfe von Expresseinstellungen kann das Problem schnell behoben werden:</span><span class="sxs-lookup"><span data-stu-id="1f60c-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="1f60c-105">[Laden Sie die neueste Version von AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771)herunter.</span><span class="sxs-lookup"><span data-stu-id="1f60c-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="1f60c-106">[Folgen Sie den Anweisungen für die Expressinstallation.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="1f60c-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="1f60c-107">Azure AD Connect muss unter Windows Server 2012 oder höher installiert sein.</span><span class="sxs-lookup"><span data-stu-id="1f60c-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="1f60c-108">Dieser Server muss der Domäne beigetreten sein und kann ein Domänencontroller oder ein Mitgliedsserver sein.</span><span class="sxs-lookup"><span data-stu-id="1f60c-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="1f60c-109">Eine vollständige Liste der Azure AD-Verbinden Anforderungen und Voraussetzungen erhalten Sie unter ["Voraussetzungen für Azure AD Verbinden."](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)</span><span class="sxs-lookup"><span data-stu-id="1f60c-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="1f60c-110">Weitere Informationen zu AADConnect-Dienstkonten finden Sie unter [Azure AD Connect: Konten und Berechtigungen](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="1f60c-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
