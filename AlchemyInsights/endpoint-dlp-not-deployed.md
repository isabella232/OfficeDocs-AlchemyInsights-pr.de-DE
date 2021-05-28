---
title: Verhinderung von Datenverlust am Endpunkt auf dem Gerät des Benutzers nicht bereitgestellt
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/27/2021
ms.locfileid: "52694806"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>Verhinderung von Datenverlust am Endpunkt auf dem Gerät des Benutzers nicht bereitgestellt

Wenn die Einstellung für die Verhinderung von Datenverlust am Endpunkt nicht auf das Gerät eines Benutzers angewendet wurde, stellen Sie sicher, dass Sie die folgenden Kriterien erfüllt sind:

- Auf dem Gerät ist Windows 10 x64, Build 1809 oder höher, installiert.
- Antischadsoftware-Client, Version 4.18.2009.7 oder höher, ist installiert.
- Auf das Gerät trifft **einer** der folgenden Punkte zu:
    
    - Es ist in Azure Active Directory (Azure AD) eingebunden
    - Es ist in Azure AD Hybrid eingebunden
    - Es ist in AAD registriert

- Um Richtlinienaktionen durchzusetzen, stellen Sie sicher, dass der Microsoft Chromium Edge-Browser auf dem Endpunktgerät installiert ist.

Weitere Anforderungen für die Bereitstellung der Verhinderung von Datenverlust am Endpunkt finden Sie unter [Erste Schritte mit der Verhinderung von Datenverlust am Endpunkt](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).