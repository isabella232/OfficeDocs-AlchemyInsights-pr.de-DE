---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: b7580f0e609d21bdc13fc07fda0bfd15bdb7a7ca
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709069"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="d0b24-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="d0b24-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="d0b24-103">Arbeiten mit PowerShell oder Skripts in Sharepoint Online?</span><span class="sxs-lookup"><span data-stu-id="d0b24-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="d0b24-104">Weitere Informationen finden Sie unter den links unten.</span><span class="sxs-lookup"><span data-stu-id="d0b24-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="d0b24-105">Erste Schritte mit der SharePoint Online-Verwaltungsshell</span><span class="sxs-lookup"><span data-stu-id="d0b24-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="d0b24-106">Herstellen einer Verbindung mit SPO PowerShell mit mehrstufiger Authentifizierung (MFA)</span><span class="sxs-lookup"><span data-stu-id="d0b24-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="d0b24-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) enthält eine Bibliothek mit PowerShell-Befehlen, mit der Sie komplexe Verwaltungsaktionen für SPO ausführen können.</span><span class="sxs-lookup"><span data-stu-id="d0b24-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="d0b24-108">Wenn Probleme bei der Verbindung mit der [SPO-Verwaltungsshell](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) auftreten, stellen Sie sicher, dass Sie auf die neueste Version aktualisiert haben, und versuchen Sie, das Modul mithilfe von *"Import-Module Microsoft.Online.SharePoint.PowerShell"* erneut zu importieren.</span><span class="sxs-lookup"><span data-stu-id="d0b24-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="d0b24-109">Wenn Sie versuchen, clientseitige Objektmodellskripts auszuführen, müssen Sie das [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) auf Ihrem lokalen Computer installiert haben.</span><span class="sxs-lookup"><span data-stu-id="d0b24-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="d0b24-110">Wenn Sie Probleme beim Ausführen von Skripts in PowerShell haben, sollten Sie die Ausführung von PowerShell als Administrator in Betracht ziehen und die [Ausführungsrichtlinie ändern.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="d0b24-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>