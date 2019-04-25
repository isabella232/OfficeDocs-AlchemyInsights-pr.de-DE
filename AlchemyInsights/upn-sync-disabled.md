---
title: UPN-Synchronisierung deaktiviert
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2a03ac64d92c07b523b015850251b33c58bb76f8
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423543"
---
# <a name="upn-sync-disabled"></a>UPN-Synchronisierung deaktiviert

Wenn Sie vor dem 30. März 2016 mit der Synchronisierung mit Azure AD begonnen haben, führen Sie das folgende Azure AD PowerShell-Cmdlet aus, um die UPN-weiche Übereinstimmung nur für Ihre Organisation zu aktivieren:
  
 **Set-MsolDirSyncFeature-Feature EnableSoftMatchOnUpn-enable $True**
  
Die UPN-weiche Übereinstimmung wird automatisch für Organisationen aktiviert, die an oder nach dem 30. März 2016 mit Azure AD synchronisiert haben.
  
Weitere Informationen zum Aktivieren von Soft Match für UPN und andere Synchronisierungsfunktionen finden Sie unter [Azure AD Connect Sync Service Features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

