---
title: Mehrere Benutzer erhalten beim Hinzufügen von Add-Ins in Outlook den Fehler „Zugriff verweigert“
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 611a4df473458abc0ab0c65442f2141763f7b868
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724362"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="df745-102">Mehrere Benutzer erhalten beim Hinzufügen von Add-Ins in Outlook den Fehler „Zugriff verweigert“</span><span class="sxs-lookup"><span data-stu-id="df745-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="df745-p101">Sie können angeben, welche Administratoren in Ihrer Organisation Berechtigungen zum Installieren und Verwalten von Add-Ins für Outlook haben. Außerdem können Sie angeben, welche Benutzer in Ihrer Organisation die Berechtigung zum Installieren und Verwalten von Add-Ins zur eigenen Verwendung besitzen.</span><span class="sxs-lookup"><span data-stu-id="df745-p101">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook. You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="df745-105">Weitere Informationen finden Sie unter [Festlegen der Administratoren und Benutzer, die Add-Ins für Outlook installieren und verwalten dürfen](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="df745-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="df745-106">Um zu überprüfen, ob Sie Berechtigungen für einen Benutzer erfolgreich zugewiesen haben, ersetzen Sie <Role Name> durch den Namen der Rolle, um dies zu verifizieren, und führen Sie den folgenden Befehl in Exchange Online PowerShell aus:</span><span class="sxs-lookup"><span data-stu-id="df745-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="df745-107">Get-ManagementRoleAssignment -Rolle „<Role Name>“ -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="df745-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="df745-108">Dieses Beispiel veranschaulicht, wie Sie verifizieren können, wem Sie Berechtigungen zum Installieren von Add-Ins aus dem Office Store für die Organisation zugewiesen haben.</span><span class="sxs-lookup"><span data-stu-id="df745-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="df745-109">PowerShell</span><span class="sxs-lookup"><span data-stu-id="df745-109">PowerShell</span></span>

<span data-ttu-id="df745-110">-Rolle „Org Marketplace-Apps“-Option GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="df745-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="df745-111">Überprüfen Sie in den Ergebnissen, Get-ManagementRoleAssignment, die Einträge in der Spalte effektive Benutzer.</span><span class="sxs-lookup"><span data-stu-id="df745-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="df745-112">Ausführliche Informationen zu Syntax und Parametern finden Sie unter [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="df745-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 