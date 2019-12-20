---
title: Microsoft Teams-4c7-Fehler
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796120"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="ba72f-102">4c7-Fehler in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ba72f-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="ba72f-103">Dieser Fehler tritt auf, weil Microsoft Teams die Formularauthentifizierung erfordert.</span><span class="sxs-lookup"><span data-stu-id="ba72f-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="ba72f-104">Wenn Sie Active Directory Verbunddienste (AD FS) bereitstellen, ist die Formularauthentifizierung standardmäßig nicht für das Intranet aktiviert.</span><span class="sxs-lookup"><span data-stu-id="ba72f-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="ba72f-105">Wenn die integrierte Windows-Authentifizierung fehlschlägt, werden Sie aufgefordert, sich mit der Formularauthentifizierung anzumelden.</span><span class="sxs-lookup"><span data-stu-id="ba72f-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="ba72f-106">Um dieses Problem zu beheben, aktivieren Sie die Formularauthentifizierung mithilfe des AD FS-MMC-Snap-Ins (Microsoft Management Console) auf dem Computer mit der lokalen Kopie von Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ba72f-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="ba72f-107">Führen Sie hierzu die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="ba72f-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="ba72f-108">Navigieren Sie im Navigationsbereich zu **Authentifizierungsrichtlinien**.</span><span class="sxs-lookup"><span data-stu-id="ba72f-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="ba72f-109">Wählen Sie im Detailbereich unter **Aktionen** die Option **globale primäre Authentifizierung bearbeiten**aus.</span><span class="sxs-lookup"><span data-stu-id="ba72f-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="ba72f-110">Wählen Sie auf der Registerkarte **Intranet** die Option **Formularauthentifizierung**aus.</span><span class="sxs-lookup"><span data-stu-id="ba72f-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="ba72f-111">Wählen Sie **OK** (oder **anwenden**) aus.</span><span class="sxs-lookup"><span data-stu-id="ba72f-111">Select **OK** (or **Apply**).</span></span>