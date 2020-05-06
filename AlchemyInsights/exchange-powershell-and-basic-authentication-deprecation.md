---
title: Die Standardauthentifizierung für Exchange PowerShell wird eingestellt
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015688"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Die Standardauthentifizierung für Exchange PowerShell wird eingestellt

Die neuesten Informationen darüber, wie eine Verbindung zu Exchange Online PowerShell ohne Verwendung der Standardauthentifizierung hergestellt werden kann, [finden Sie hier](https://aka.ms/psbasicauth).

Beachten Sie, dass auf dem Clientcomputer weiterhin die Standardauthentifizierung aktiviert sein muss.
Das neue PowerShell V2-Modul verwendet moderne Authentifizierung, um eine Verbindung zum Aktivieren aller REST-basierten V2-Cmdlets herzustellen. Zusätzlich zu den V2-Cmdlets ermöglicht es Ihnen auch den Zugriff auf ältere Remote-PowerShell-Cmdlets (RPS), für die eine PowerShell-Remotesitzung eingerichtet werden muss. Zum Einrichten einer RPS-Sitzung auf einem Windows-Computer muss WinRM BasicAuth auf dem Clientcomputer aktiviert werden, auch wenn das Modul einen modernen Authentifizierungsmechanismus für den Dienst verwendet. Die WinRM-Standardauthentifizierungspipeline wird für den Transport moderner Authentifizierungstoken verwendet. Wenn die WinRM-Standardauthentifizierung auf dem Clientcomputer deaktiviert ist, funktionieren die neuen V2-Cmdlets weiterhin (aber die alten RPS-Cmdlets nicht).
