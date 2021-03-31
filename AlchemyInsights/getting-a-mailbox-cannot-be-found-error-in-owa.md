---
title: 126 Fehler beim Abrufen eines Postfachs in OWA gefunden?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426661"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="1e7e6-102">Abrufen eines Postfachs nicht gefunden Fehler in Outlook im Web?</span><span class="sxs-lookup"><span data-stu-id="1e7e6-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="1e7e6-103">Wenn Sie Outlook im Web verwenden und ein **Postfach** nicht gefunden werden konnte, ist das Konto, das Sie zum Herstellen einer Verbindung mit Outlook im Web verwendet haben, nicht über eine Exchange Online-Lizenz, und daher ist dem Konto kein Postfach zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="1e7e6-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="1e7e6-104">Ihr Administrator kann Ihrem Konto eine Lizenz zuweisen, indem sie die folgenden Schritte ausführen:</span><span class="sxs-lookup"><span data-stu-id="1e7e6-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="1e7e6-105">Öffnen Sie [das Microsoft 365 Admin Center,](https://portal.office.com/adminportal/home#/homepage) und wechseln Sie im Abschnitt Benutzer zu Aktive Benutzer, und wählen Sie den Benutzer aus, dem der Fehler angezeigt wird.  </span><span class="sxs-lookup"><span data-stu-id="1e7e6-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="1e7e6-106">Wechseln Sie auf der geöffneten Benutzerseite zum Abschnitt Lizenzen und **Apps,** wählen Sie den entsprechenden **Standortwert** aus, und weisen Sie eine Lizenz zu, die Exchange Online enthält (erweitern Sie die Lizenz, um ihre Details anzuzeigen).</span><span class="sxs-lookup"><span data-stu-id="1e7e6-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="1e7e6-107">Klicken Sie nach Abschluss des Vorgangs auf **Änderungen speichern**.</span><span class="sxs-lookup"><span data-stu-id="1e7e6-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="1e7e6-108">In einigen Fällen hilft das Entfernen und Erneute Zuweisen der Lizenz, wenn die Lizenz bereits einem Benutzerkonto zugewiesen ist, das Problem zu beheben und ordnungsgemäß im System bereitgestellt zu bekommen:</span><span class="sxs-lookup"><span data-stu-id="1e7e6-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="1e7e6-109">Überprüfen Sie, ob Ihre M365 Exchange Online -Abonnements (und andere, sofern Sie über ein Abonnement verfügen) aktuell sind und noch nicht abgelaufen sind.</span><span class="sxs-lookup"><span data-stu-id="1e7e6-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="1e7e6-110">Nachdem Sie sichergestellt haben, dass Ihr Abonnement nicht abgelaufen ist und dem Benutzerkonto eine gültige Lizenz zugewiesen wurde, kann es bis zu 24 Stunden dauern, bis die Lizenz bereitgestellt wurde, sodass Sie möglicherweise warten müssen, bis Ihr Problem behoben ist.</span><span class="sxs-lookup"><span data-stu-id="1e7e6-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="1e7e6-111">Weitere Informationen finden Sie unter [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span><span class="sxs-lookup"><span data-stu-id="1e7e6-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>