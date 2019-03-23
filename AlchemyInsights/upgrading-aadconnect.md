---
title: 932 Upgrade von AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 0bbb847bb1381330065ebba6e109795908b06490
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/22/2019
ms.locfileid: "30778741"
---
# <a name="upgrade-azure-ad-connect"></a>Aktualisieren von Azure AD Connect

Standardmäßig ist das automatische Upgrade für Azure AD Connect aktiviert, sodass Sie sicherstellen können, dass Sie die neueste Version ausführen. Verwenden Sie das Cmdlet **Get-ADSyncAutoUpgrade** in Azure AD PowerShell, um die Einstellungen für das automatische Upgrade zu überprüfen. Das Cmdlet gibt einen der folgenden Werte zurück: 
  
- **Enabled**: Automatisches Upgrade ist aktiviert. 
    
- **Deaktiviert**: Automatisches Upgrade ist deaktiviert. 
    
- **Angehalten**: das System kann keine automatischen Upgrades mehr erhalten. Sie können diesen Wert nicht konfigurieren. Sie wird vom System festgelegt. 
    
Weitere Informationen finden Sie unter [Automatisches Upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).
  
Um die neueste Version von Azure AD Connect herunterzuladen, wechseln [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)Sie zu.
  

