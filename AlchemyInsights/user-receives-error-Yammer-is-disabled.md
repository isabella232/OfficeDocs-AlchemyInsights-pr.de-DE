---
title: 'Benutzer erhält den Fehler: AADSTS7000112 Yammer ist deaktiviert'
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45157296"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="d7ef2-102">Benutzer erhält den Fehler: AADSTS7000112 Yammer ist deaktiviert</span><span class="sxs-lookup"><span data-stu-id="d7ef2-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="d7ef2-103">Wenn die Fehlermeldung "AADSTS7000112: Anwendung '00000005-0000-0ff1-ce00-000000000000' (Yammer) ist deaktiviert" angezeigt wird, liegt ein Problem mit dem Dienstprinzipal in Azure AD vor.</span><span class="sxs-lookup"><span data-stu-id="d7ef2-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="d7ef2-104">Möglicherweise hat ein Administrator den Dienstprinzipal deaktiviert, um den Zugriff auf Yammer zu blockieren.</span><span class="sxs-lookup"><span data-stu-id="d7ef2-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="d7ef2-105">Das Deaktivieren des Dienstprinzipals wird nicht empfohlen und kann zu weiteren Problemen führen.</span><span class="sxs-lookup"><span data-stu-id="d7ef2-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="d7ef2-106">Weitere Informationen zum unterstützten Ansatz für dass Blockieren des Benutzerzugriffs auf Yammer finden Sie unter [Deaktivieren des Zugriffs auf Yammer für Microsoft 365-Benutzer](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="d7ef2-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="d7ef2-107">So beheben Sie dieses Problem im Azure-Portal und stellen den Benutzerzugriffs auf Yammer wieder her</span><span class="sxs-lookup"><span data-stu-id="d7ef2-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="d7ef2-108">Öffnen Sie die Azure Active Directory-Seite, und wählen Sie im linken Navigationsbereich **Enterprise-Anwendungen** unter **Verwalten** aus.</span><span class="sxs-lookup"><span data-stu-id="d7ef2-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="d7ef2-109">Geben Sie **Office 365 Yammer** in das Suchfeld ein, und wählen Sie den Namen der Anwendung aus, um die Einstellungen zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="d7ef2-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="d7ef2-110">Wählen Sie im linken Navigationsbereich unter **Eigenschaften\*\*\*\*Verwalten** aus.</span><span class="sxs-lookup"><span data-stu-id="d7ef2-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="d7ef2-111">Legen Sie den Wert für **Für Benutzeranmeldung aktiviert?** auf **Ja** fest, und wählen Sie dann **Speichern** aus.</span><span class="sxs-lookup"><span data-stu-id="d7ef2-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="d7ef2-112">Melden Sie sich wieder bei Yammer an.</span><span class="sxs-lookup"><span data-stu-id="d7ef2-112">Sign in to Yammer again.</span></span> <span data-ttu-id="d7ef2-113">Möglicherweise müssen Sie Cookies löschen.</span><span class="sxs-lookup"><span data-stu-id="d7ef2-113">You might need to clear cookies.</span></span>

<span data-ttu-id="d7ef2-114">Alternativ können Sie den Wert unter Verwendung von PowerShell-Befehlen festlegen.</span><span class="sxs-lookup"><span data-stu-id="d7ef2-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="d7ef2-115">Weitere Informationen finden Sie unter [Fehler "Leider können wir Sie nicht anmelden" beim Klicken auf die Yammer-Kachel in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="d7ef2-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 