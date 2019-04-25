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
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389680"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="c22a3-102">Aktualisieren von Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="c22a3-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="c22a3-103">Standardmäßig ist das automatische Upgrade für Azure AD Connect aktiviert, sodass Sie sicherstellen können, dass Sie die neueste Version ausführen.</span><span class="sxs-lookup"><span data-stu-id="c22a3-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="c22a3-104">Verwenden Sie das Cmdlet **Get-ADSyncAutoUpgrade** in Azure AD PowerShell, um die Einstellungen für das automatische Upgrade zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="c22a3-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="c22a3-105">Das Cmdlet gibt einen der folgenden Werte zurück:</span><span class="sxs-lookup"><span data-stu-id="c22a3-105">The cmdlet will return one of following values:</span></span> 

- <span data-ttu-id="c22a3-106">**Enabled**: Automatisches Upgrade ist aktiviert.</span><span class="sxs-lookup"><span data-stu-id="c22a3-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="c22a3-107">**Deaktiviert**: Automatisches Upgrade ist deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="c22a3-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="c22a3-108">**Angehalten**: das System kann keine automatischen Upgrades mehr erhalten.</span><span class="sxs-lookup"><span data-stu-id="c22a3-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="c22a3-109">Sie können diesen Wert nicht konfigurieren. Sie wird vom System festgelegt.</span><span class="sxs-lookup"><span data-stu-id="c22a3-109">You can't configure this value; it's set by the system.</span></span> 

<span data-ttu-id="c22a3-110">Weitere Informationen finden Sie unter [Automatisches Upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="c22a3-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="c22a3-111">Um die neueste Version von Azure AD Connect herunterzuladen, wechseln [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)Sie zu.</span><span class="sxs-lookup"><span data-stu-id="c22a3-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
