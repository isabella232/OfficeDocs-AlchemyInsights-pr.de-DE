---
title: Mehreren Benutzern werden keine Add-Ins in Outlook angezeigt
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729870"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="62dbb-102">Mehreren Benutzern werden keine Add-Ins in Outlook angezeigt</span><span class="sxs-lookup"><span data-stu-id="62dbb-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="62dbb-103">Wenn Sie Outlook-Add-Ins testen und keine angezeigt werden, verwenden Sie als ersten Schritt zur Problembehandlung das PowerShell-Cmdlet **Get-OrganizationConfig**, um den Parameter _AppsForOffice Enabled_ abzufragen.</span><span class="sxs-lookup"><span data-stu-id="62dbb-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="62dbb-104">Wenn die Abfrage den Wert **False** zurückgibt, setzen Sie diesen Parameter mit dem Cmdlet **Set-OrganizationConfig** auf **True**, damit Add-Ins wie erwartet angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="62dbb-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="62dbb-105">Es wird nicht empfohlen, den Parameter _AppsForOfficeEnabled_ auf **False** zu setzen.</span><span class="sxs-lookup"><span data-stu-id="62dbb-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="62dbb-106">Der Wert **False**setzt alle vorstehenden Administrator- und Benutzerrolleneinstellungen außer Kraft und verhindert, dass neue Apps von einem Benutzer in der Organisation aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="62dbb-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="62dbb-107">Weitere Informationen finden Sie unter [Festlegen der Administratoren und Benutzer, die Add-Ins für Outlook installieren und verwalten dürfen](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="62dbb-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>