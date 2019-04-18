---
title: Beheben von e-Mail-Übermittlungsproblemen für e-Mail-aktivierte Öffentliche Ordner
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: d1c1d5bcb52ba9083e8dd7603feb72436c5154c8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/17/2019
ms.locfileid: "31910597"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="59bbe-102">Beheben von e-Mail-Übermittlungsproblemen für e-Mail-aktivierte Öffentliche Ordner</span><span class="sxs-lookup"><span data-stu-id="59bbe-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="59bbe-103">Wenn externe Absender keine Nachrichten an Ihre e-Mail-aktivierten Öffentlichen Ordner senden können und die Absender den Fehler erhalten: wurde **nicht gefunden (550 5.4.1)**, überprüfen Sie, ob die e-Mail-Domäne für den öffentlichen Ordner als interne Relay-Domäne anstelle eines autorisierende Domäne:</span><span class="sxs-lookup"><span data-stu-id="59bbe-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="59bbe-104">Öffnen Sie das [Exchange Admin Center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="59bbe-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="59bbe-105">Wechseln Sie zu **akzeptierte Domänen**für den **Nachrichtenfluss** \> , wählen Sie die akzeptierte Domäne aus, und klicken Sie dann auf **Bearbeiten**.</span><span class="sxs-lookup"><span data-stu-id="59bbe-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="59bbe-106">Ändern Sie auf der Eigenschaftenseite, die geöffnet wird, wenn der Domänentyp auf **autorisierend**festgelegt ist, den Wert in **Internes Relay** , und klicken Sie dann auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="59bbe-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="59bbe-107">Wenn externe Absender die Fehlermeldung erhalten, die **Sie nicht über die Berechtigung verfügen (550 5.7.13)**, führen Sie den folgenden Befehl in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) aus, um die Berechtigungen für anonyme Benutzer im öffentlichen Ordner anzuzeigen:</span><span class="sxs-lookup"><span data-stu-id="59bbe-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="59bbe-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Beispiel: `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="59bbe-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="59bbe-109">Damit externe Benutzer e-Mails an diesen öffentlichen Ordner senden können, fügen Sie dem Benutzer anonymous das Zugriffsrecht createItems hinzu.</span><span class="sxs-lookup"><span data-stu-id="59bbe-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="59bbe-110">Beispiel: `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="59bbe-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
