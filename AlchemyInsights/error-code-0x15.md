---
title: Fehlercode 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Fehler beim Aktivieren von Office 2013 auf Remote Desktop Services (RDS) Bereitstellungen empfangen werden, sollten Sie ADAL durch Bearbeiten der Registrierung aktivieren.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29929087"
---
<span data-ttu-id="b2ecd-103">Fehler beim Aktivieren von Office 2013 auf Remote Desktop Services (RDS) Bereitstellungen empfangen werden, sollten Sie ADAL durch Bearbeiten der Registrierung aktivieren.</span><span class="sxs-lookup"><span data-stu-id="b2ecd-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="b2ecd-104">**Registrierungsschlüssel**</span><span class="sxs-lookup"><span data-stu-id="b2ecd-104">**Registry key**</span></span>|<span data-ttu-id="b2ecd-105">**Typ**</span><span class="sxs-lookup"><span data-stu-id="b2ecd-105">**Type**</span></span>|<span data-ttu-id="b2ecd-106">**Wert**</span><span class="sxs-lookup"><span data-stu-id="b2ecd-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b2ecd-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="b2ecd-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="b2ecd-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="b2ecd-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="b2ecd-109">1</span><span class="sxs-lookup"><span data-stu-id="b2ecd-109">1</span></span>  <br/> |
   
<span data-ttu-id="b2ecd-110">Weitere Informationen finden Sie unter [Modernen Authentifizierung für Office 2013 auf Windows-Geräten aktivieren](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="b2ecd-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="b2ecd-p101">ADAL ist in Office 365 ProPlus und Office 2016 standardmäßig aktiviert. > remote Desktop Services (RDS) wurde zuvor Terminaldienste bezeichnet.</span><span class="sxs-lookup"><span data-stu-id="b2ecd-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

