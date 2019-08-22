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
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="4c26d-102">Upgrade Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="4c26d-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="4c26d-103">Standardmäßig ist das automatische Upgrade für Azure AD Connect aktiviert, sodass Sie sicherstellen können, dass Sie die neueste Version ausgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="4c26d-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="4c26d-104">Verwenden Sie das Cmdlet **Get-ADSyncAutoUpgrade** in Azure AD PowerShell, um die Einstellungen für das automatische Upgrade zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="4c26d-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="4c26d-105">Das Cmdlet gibt einen der folgenden Werte zurück:</span><span class="sxs-lookup"><span data-stu-id="4c26d-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="4c26d-106">**Aktiviert**: das automatische Upgrade ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="4c26d-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="4c26d-107">**Deaktiviert**: das automatische Upgrade ist deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="4c26d-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="4c26d-108">**Angehalten**: das System ist nicht mehr berechtigt, automatische Upgrades zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="4c26d-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="4c26d-109">Sie können diesen Wert nicht konfigurieren. Sie wird vom System festgelegt.</span><span class="sxs-lookup"><span data-stu-id="4c26d-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="4c26d-110">Weitere Informationen finden Sie unter [Automatisches Upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="4c26d-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="4c26d-111">Um die neueste Version von Azure AD Connect herunterzuladen, wechseln [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)Sie zu.</span><span class="sxs-lookup"><span data-stu-id="4c26d-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
