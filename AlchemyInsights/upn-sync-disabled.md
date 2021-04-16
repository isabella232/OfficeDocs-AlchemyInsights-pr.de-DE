---
title: UPN-Synchronisierung deaktiviert
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782150"
---
# <a name="upn-sync-disabled"></a>UPN-Synchronisierung deaktiviert

Wenn Sie mit der Synchronisierung mit Azure AD vor dem 30. März 2016 begonnen haben, führen Sie das folgende Azure AD PowerShell-Cmdlet aus, um nur die softe UpN-Übereinstimmung für Ihre Organisation zu aktivieren:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
Die weiche UPN-Übereinstimmung wird automatisch für Organisationen aktiviert, die mit der Synchronisierung mit Azure AD am oder nach dem 30. März 2016 begonnen haben.
  
Weitere Informationen zum Aktivieren einer weichen Übereinstimmung auf UPN und anderen Synchronisierungsfeatures finden Sie unter [Azure AD Connect-Synchronisierungsdienstfeatures](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

