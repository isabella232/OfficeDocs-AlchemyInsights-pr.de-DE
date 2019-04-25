---
title: Fehler Code 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Wenn beim Aktivieren von Office 2013 in Remote Desktop Dienste-Bereitstellungen eine Fehlermeldung angezeigt wird, sollten Sie die Aktivierung von ADAL durch Bearbeiten der Registrierung erwägen.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402738"
---
<span data-ttu-id="3b6e7-103">Wenn beim Aktivieren von Office 2013 in Remote Desktop Dienste-Bereitstellungen eine Fehlermeldung angezeigt wird, sollten Sie die Aktivierung von ADAL durch Bearbeiten der Registrierung erwägen.</span><span class="sxs-lookup"><span data-stu-id="3b6e7-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="3b6e7-104">**Registrierungsschlüssel**</span><span class="sxs-lookup"><span data-stu-id="3b6e7-104">**Registry key**</span></span>|<span data-ttu-id="3b6e7-105">**Typ**</span><span class="sxs-lookup"><span data-stu-id="3b6e7-105">**Type**</span></span>|<span data-ttu-id="3b6e7-106">**Wert**</span><span class="sxs-lookup"><span data-stu-id="3b6e7-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3b6e7-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="3b6e7-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="3b6e7-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="3b6e7-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="3b6e7-109">1 </span><span class="sxs-lookup"><span data-stu-id="3b6e7-109">1</span></span>  <br/> |
   
<span data-ttu-id="3b6e7-110">Weitere Informationen finden Sie unter [Aktivieren der modernen Authentifizierung für Office 2013 auf Windows-Geräten](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="3b6e7-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="3b6e7-111">ADAL ist in Office 365 proPlus und Office 2016 standardmäßig aktiviert.</span><span class="sxs-lookup"><span data-stu-id="3b6e7-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="3b6e7-112">> Remote Desktop Dienste (RDS) wurde zuvor als Terminal Dienste bezeichnet.</span><span class="sxs-lookup"><span data-stu-id="3b6e7-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

