---
title: Fehler Code 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Wenn beim Aktivieren von Office 2013 für Remote Desktop Dienste (RDS)-Bereitstellungen ein Fehler auftritt, sollten Sie Adal durch Bearbeiten der Registrierung aktivieren.
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36526992"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="3856b-103">Fehler bei Aktivierung Office 2013 für Remote Desktop Dienste</span><span class="sxs-lookup"><span data-stu-id="3856b-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="3856b-104">Wenn beim Aktivieren von Office 2013 für Remote Desktop Dienste (RDS)-Bereitstellungen ein Fehler auftritt, sollten Sie Adal durch Bearbeiten der Registrierung aktivieren.</span><span class="sxs-lookup"><span data-stu-id="3856b-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="3856b-105">**Registrierungsschlüssel**</span><span class="sxs-lookup"><span data-stu-id="3856b-105">**Registry key**</span></span>|<span data-ttu-id="3856b-106">**Typ**</span><span class="sxs-lookup"><span data-stu-id="3856b-106">**Type**</span></span>|<span data-ttu-id="3856b-107">**Wert**</span><span class="sxs-lookup"><span data-stu-id="3856b-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3856b-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="3856b-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="3856b-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="3856b-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="3856b-110">1</span><span class="sxs-lookup"><span data-stu-id="3856b-110">1</span></span>  <br/> |

<span data-ttu-id="3856b-111">Weitere Informationen finden Sie unter [Aktivieren der modernen Authentifizierung für Office 2013 auf Windows-Geräten](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="3856b-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="3856b-112">Adal ist in Office 365 ProPlus und Office 2016 standardmäßig aktiviert.</span><span class="sxs-lookup"><span data-stu-id="3856b-112">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="3856b-113">Remote Desktop Dienste (RDS) hießen zuvor Terminal Dienste.</span><span class="sxs-lookup"><span data-stu-id="3856b-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  