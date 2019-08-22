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
ms.openlocfilehash: f390d659b191fa4c44bd7c8acb32409cd3021489
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36532330"
---
# <a name="upn-sync-disabled"></a>UPN-Synchronisierung deaktiviert

Wenn Sie mit der Synchronisierung mit Azure AD vor dem 30. März 2016 begonnen haben, führen Sie das folgende Azure AD PowerShell-Cmdlet aus, um UPN Soft Match nur für Ihre Organisation zu aktivieren:
  
 **Festlegen-MsolDirSyncFeature-Feature EnableSoftMatchOnUpn-enable $true**
  
UPN Soft Match wird automatisch für Organisationen aktiviert, die mit der Synchronisierung mit Azure AD begonnen haben oder nach dem 30. März 2016.
  
Weitere Informationen zum Aktivieren von Soft Match unter UPN und anderen Synchronisierungsfeatures finden Sie unter [Azure AD Connect Sync Service Features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

