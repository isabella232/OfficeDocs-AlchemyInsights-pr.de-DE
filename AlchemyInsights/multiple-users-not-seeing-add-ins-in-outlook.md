---
title: Mehreren Benutzern werden keine Add-Ins in Outlook angezeigt
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45154580"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="82566-102">Mehreren Benutzern werden keine Add-Ins in Outlook angezeigt</span><span class="sxs-lookup"><span data-stu-id="82566-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="82566-103">Wenn Sie Outlook-Add-Ins testen und keine angezeigt werden, verwenden Sie als ersten Schritt zur Problembehandlung das PowerShell-Cmdlet **Get-OrganizationConfig**, um den Parameter _AppsForOffice Enabled_ abzufragen.</span><span class="sxs-lookup"><span data-stu-id="82566-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="82566-104">Wenn die Abfrage den Wert **False** zurückgibt, setzen Sie diesen Parameter mit dem Cmdlet **Set-OrganizationConfig** auf **True**, damit Add-Ins wie erwartet angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="82566-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="82566-105">Es wird nicht empfohlen, den Parameter _AppsForOfficeEnabled_ auf **False** zu setzen.</span><span class="sxs-lookup"><span data-stu-id="82566-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="82566-106">Der Wert **False**setzt alle vorstehenden Administrator- und Benutzerrolleneinstellungen außer Kraft und verhindert, dass neue Apps von einem Benutzer in der Organisation aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="82566-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="82566-107">Weitere Informationen finden Sie unter [Festlegen der Administratoren und Benutzer, die Add-Ins für Outlook installieren und verwalten dürfen](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="82566-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>