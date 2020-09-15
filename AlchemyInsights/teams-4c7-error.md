---
title: Microsoft Teams-4c7-Fehler
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700202"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="1c577-102">4c7-Fehler in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="1c577-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="1c577-103">Dieser Fehler tritt auf, weil Microsoft Teams die Formularauthentifizierung erfordert.</span><span class="sxs-lookup"><span data-stu-id="1c577-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="1c577-104">Wenn Sie Active Directory Verbunddienste (AD FS) bereitstellen, ist die Formularauthentifizierung standardmäßig nicht für das Intranet aktiviert.</span><span class="sxs-lookup"><span data-stu-id="1c577-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="1c577-105">Wenn die integrierte Windows-Authentifizierung fehlschlägt, werden Sie aufgefordert, sich mit der Formularauthentifizierung anzumelden.</span><span class="sxs-lookup"><span data-stu-id="1c577-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="1c577-106">Um dieses Problem zu beheben, aktivieren Sie die Formularauthentifizierung mithilfe des AD FS-MMC-Snap-Ins (Microsoft Management Console) auf dem Computer mit der lokalen Kopie von Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1c577-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="1c577-107">Gehen Sie dazu wie folgt vor:</span><span class="sxs-lookup"><span data-stu-id="1c577-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="1c577-108">Navigieren Sie im Navigationsbereich zu **Authentifizierungsrichtlinien**.</span><span class="sxs-lookup"><span data-stu-id="1c577-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="1c577-109">Wählen Sie im Detailbereich unter **Aktionen** die Option **globale primäre Authentifizierung bearbeiten**aus.</span><span class="sxs-lookup"><span data-stu-id="1c577-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="1c577-110">Wählen Sie auf der Registerkarte **Intranet** die Option **Formularauthentifizierung**aus.</span><span class="sxs-lookup"><span data-stu-id="1c577-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="1c577-111">Wählen Sie **OK** (oder **anwenden**) aus.</span><span class="sxs-lookup"><span data-stu-id="1c577-111">Select **OK** (or **Apply**).</span></span>