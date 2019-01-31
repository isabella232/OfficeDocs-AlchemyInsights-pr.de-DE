---
title: UPN-Synchronisierung deaktiviert
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 027782bb2a6b892df6201f3c3bf55151ef7b9db7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657970"
---
# <a name="upn-sync-disabled"></a>UPN-Synchronisierung deaktiviert

Wenn Sie Azure AD vor dem 30 März 2016 Synchronisierung gestartet führen Sie das folgende Azure AD-PowerShell-Cmdlet, um weiche UPN-Übereinstimmung für Ihre Organisation nur zu aktivieren:
  
 **Set-MsolDirSyncFeature-Feature EnableSoftMatchOnUpn-$True aktivieren**
  
Weiche Übereinstimmung UPN ist automatisch für Organisationen eingeschaltet, die an oder nach 30 März 2016 Azure AD synchronisiert wird gestartet.
  
Weitere Informationen zum Aktivieren der weiche Übereinstimmung UPN und andere Synchronisierung Features, finden Sie unter [Verbinden von Azure Active Directory Sync Service-Features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

