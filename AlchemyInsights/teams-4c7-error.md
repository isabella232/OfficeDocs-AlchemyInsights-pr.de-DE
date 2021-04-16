---
title: Fehler "Teams 4c7"
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
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786668"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="686dc-102">4c7-Fehler in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="686dc-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="686dc-103">Dieser Fehler tritt auf, weil Microsoft Teams die Formularauthentifizierung erfordert.</span><span class="sxs-lookup"><span data-stu-id="686dc-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="686dc-104">Wenn Sie Active Directory Federation Services (AD FS) bereitstellen, ist die Formularauthentifizierung für das Intranet standardmäßig nicht aktiviert.</span><span class="sxs-lookup"><span data-stu-id="686dc-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="686dc-105">Wenn bei der integrierten Windows-Authentifizierung ein Fehler auftritt, werden Sie aufgefordert, sich mithilfe der Formularauthentifizierung zu anmelden.</span><span class="sxs-lookup"><span data-stu-id="686dc-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="686dc-106">Aktivieren Sie die Formularauthentifizierung mithilfe des AD FS Microsoft Management Console (MMC)-Snap-Ins auf dem Computer mit der lokalen Kopie von Active Directory, um dieses Problem zu beheben.</span><span class="sxs-lookup"><span data-stu-id="686dc-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="686dc-107">Gehen Sie dazu wie folgt vor:</span><span class="sxs-lookup"><span data-stu-id="686dc-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="686dc-108">Navigieren Sie im Navigationsbereich zu **Authentifizierungsrichtlinien**.</span><span class="sxs-lookup"><span data-stu-id="686dc-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="686dc-109">Wählen **Sie unter Aktionen** im Detailbereich die Option Globale primäre **Authentifizierung bearbeiten aus.**</span><span class="sxs-lookup"><span data-stu-id="686dc-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="686dc-110">Wählen Sie **auf der Registerkarte Intranet** die Option **Formularauthentifizierung aus.**</span><span class="sxs-lookup"><span data-stu-id="686dc-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="686dc-111">Wählen **Sie OK** (oder **Anwenden) aus.**</span><span class="sxs-lookup"><span data-stu-id="686dc-111">Select **OK** (or **Apply**).</span></span>