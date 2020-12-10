---
title: Ändern von Microsoft Edge mithilfe von Datenverzeichnis Variablen anstelle von hartcodierten Pfaden
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608844"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a><span data-ttu-id="6b306-102">Ändern von Microsoft Edge mithilfe von Datenverzeichnis Variablen anstelle von hartcodierten Pfaden</span><span class="sxs-lookup"><span data-stu-id="6b306-102">Modify Microsoft Edge by using data directory variables rather than hardcoded paths</span></span>

<span data-ttu-id="6b306-103">Wenn Sie beispielsweise in Windows die Profildaten unter den lokalen Anwendungsdaten eines Benutzers anstatt am Standardspeicherort speichern möchten, legen Sie die **UserDataDir** -Richtlinie auf **$ {local_app_data} \Edge\Profile**.</span><span class="sxs-lookup"><span data-stu-id="6b306-103">For example, on Windows, to store the profile data under a user's local application data rather than in the default location, set the **UserDataDir** policy to **${local_app_data}\Edge\Profile**.</span></span> 

<span data-ttu-id="6b306-104">Weitere Informationen finden Sie unter [Create Microsoft Edge User Data Directory variables](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).</span><span class="sxs-lookup"><span data-stu-id="6b306-104">To learn more, see [Create Microsoft Edge user data directory variables](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).</span></span>