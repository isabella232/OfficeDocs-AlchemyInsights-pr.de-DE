---
title: 932 Upgraden von AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: ff3f74348599788edd8ce0991fe49bb6a54b55af
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506082"
---
# <a name="upgrade-azure-ad-connect"></a>Upgrade Azure AD Connect

Standardmäßig ist das automatische Upgrade für Azure AD Connect aktiviert, sodass Sie sicherstellen können, dass Sie die neueste Version ausgeführt haben. Verwenden Sie das Cmdlet **Get-ADSyncAutoUpgrade** in Azure AD PowerShell, um die Einstellungen für das automatische Upgrade zu überprüfen. Das Cmdlet gibt einen der folgenden Werte zurück:

- **Aktiviert**: das automatische Upgrade ist aktiviert.

- **Deaktiviert**: das automatische Upgrade ist deaktiviert.

- **Angehalten**: das System ist nicht mehr berechtigt, automatische Upgrades zu erhalten. Sie können diesen Wert nicht konfigurieren. Sie wird vom System festgelegt.

Weitere Informationen finden Sie unter [Automatisches Upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Um die neueste Version von Azure AD Connect herunterzuladen, wechseln [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)Sie zu.
