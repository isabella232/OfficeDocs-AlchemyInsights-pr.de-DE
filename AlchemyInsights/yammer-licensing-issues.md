---
title: Probleme mit Yammer-Lizenzen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657275"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="1dd69-102">Probleme mit Yammer-Lizenzen</span><span class="sxs-lookup"><span data-stu-id="1dd69-102">Yammer licensing issues</span></span>

<span data-ttu-id="1dd69-103">Jeder Benutzer muss über eine Lizenz verfügen, um den Yammer Enterprise-Dienst zu nutzen, aber Yammer verlangt nicht standardmäßig, dass Benutzer eine Lizenz für den Zugriff auf den Dienst haben.</span><span class="sxs-lookup"><span data-stu-id="1dd69-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="1dd69-104">Wenn ein Administrator die Einstellung ändert, um Microsoft 365-Benutzer ohne Yammer-Lizenzen zu blockieren, können Benutzer, denen keine Yammer Enterprise-Lizenz zugewiesen wurde, auf den Yammer-Dienst nicht zugreifen.</span><span class="sxs-lookup"><span data-stu-id="1dd69-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="1dd69-105">Weitere Informationen finden Sie unter [Verwalten von Yammer-Benutzerlizenzen in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="1dd69-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="1dd69-106">Wenn Benutzern Lizenzen entzogen werden, wird die Yammer-Kachel nicht mehr angezeigt, und andere Dienste können die Lizenzentfernung nutzen, um Features auszublenden.</span><span class="sxs-lookup"><span data-stu-id="1dd69-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="1dd69-107">In anderen Fällen werden die Features zwar weiterhin angezeigt, zum Verwenden der Features muss aber eine Lizenz zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="1dd69-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="1dd69-108">**Die Lizenz wird für den Benutzer nicht aktualisiert**</span><span class="sxs-lookup"><span data-stu-id="1dd69-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="1dd69-109">Gelegentlich wurde einem Benutzer eine Lizenz zugewiesen, aber er kann trotzdem nicht auf Yammer zugreifen.</span><span class="sxs-lookup"><span data-stu-id="1dd69-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="1dd69-110">Verzögerungen treten eher auf, wenn eine Massenlizenzzuweisung in Bearbeitung ist.</span><span class="sxs-lookup"><span data-stu-id="1dd69-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="1dd69-111">Yammer-Benutzer werden möglicherweise nicht in derselben Reihenfolge aktualisiert wie Lizenzen in Azure AD geändert werden, da das System asynchron ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="1dd69-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="1dd69-112">Warten Sie bis zu 24 Stunden, bevor Sie einen Supportfall öffnen, um Probleme mit der Synchronisierung von Lizenzen zu melden.</span><span class="sxs-lookup"><span data-stu-id="1dd69-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="1dd69-113">**Massenzuweisung von Lizenzen**</span><span class="sxs-lookup"><span data-stu-id="1dd69-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="1dd69-114">Lizenzen können über das Admin Center oder PowerShell-Skripts zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="1dd69-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="1dd69-115">Weitere Informationen finden Sie unter [Zuweisen von Lizenzen an Benutzer](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) und [Zuweisen von Lizenzen zu Benutzerkonten mit Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="1dd69-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="1dd69-116">Der Microsoft-Support bietet keine Unterstützung beim Erstellen von Skripts, aber Dokumentation zu Yammer-Lizenzzuweisungen steht zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="1dd69-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="1dd69-117">Weitere Informationen finden Sie unter [Verwalten von Yammer-Lizenzen mit Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="1dd69-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>