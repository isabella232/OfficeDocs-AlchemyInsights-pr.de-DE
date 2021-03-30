---
title: Azure Active Directory-Beitritt
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403798"
---
# <a name="azure-active-directory-join"></a><span data-ttu-id="c9845-102">Azure Active Directory-Beitritt</span><span class="sxs-lookup"><span data-stu-id="c9845-102">Azure Active Directory join</span></span>

1. <span data-ttu-id="c9845-103">Wenn Sie geräteregistrierungen zum ersten Mal einrichten, stellen Sie sicher, dass Sie die Einführung in die Geräteverwaltung [in Azure Active Directory](/azure/active-directory/devices/overview) überprüft haben, die Sie bei der Bereitstellung von Geräten in Azure AD unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c9845-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="c9845-104">Wenn Sie Geräte direkt bei Azure AD registrieren und sie bei Intune registrieren, müssen Sie [](/mem/intune/fundamentals/licenses-assign) sicherstellen, dass Sie [Intune](/mem/intune/enrollment/device-enrollment) konfiguriert haben und zuerst die Lizenzierung haben.</span><span class="sxs-lookup"><span data-stu-id="c9845-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](/mem/intune/enrollment/device-enrollment) and have the [licensing](/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="c9845-105">Stellen Sie sicher, dass Sie autorisiert sind, Vorgänge in Azure AD durchzuführen.</span><span class="sxs-lookup"><span data-stu-id="c9845-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="c9845-106">Nur ein globaler Administrator in Azure AD kann Einstellungen für Geräteregistrierungen verwalten.</span><span class="sxs-lookup"><span data-stu-id="c9845-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="c9845-107">Informationen zur Azure AD-Beitrittsimplementierung finden Sie unter [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span><span class="sxs-lookup"><span data-stu-id="c9845-107">To do Azure AD join implementation, see [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="c9845-108">Weitere Informationen zum Beheben gängiger Probleme bei der Azure AD-Teilnahme finden Sie unter Häufig gestellte Fragen zur [Azure Ad-Teilnahme](/azure/active-directory/devices/faq) und für Windows 10 Pro-Geräte unter Nicht in der Lage, [Windows 10 Pro-Computer zu Azure AD](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)zu verbinden – Müssen auf aktualisieren – Microsoft Community .</span><span class="sxs-lookup"><span data-stu-id="c9845-108">For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span></span>
