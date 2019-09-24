---
title: SharePoint Online PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 00ec337ce34da9d3c3fba0a71602c3078a556552
ms.sourcegitcommit: 6b102e079a7d30298105fd811a67efb707d6d5bf
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/23/2019
ms.locfileid: "37122998"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="bf8d1-102">SharePoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="bf8d1-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="bf8d1-103">Arbeiten mit PowerShell oder Skripts in SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="bf8d1-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="bf8d1-104">Weitere Informationen finden Sie unter den folgenden Links.</span><span class="sxs-lookup"><span data-stu-id="bf8d1-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="bf8d1-105">Erste Schritte mit SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="bf8d1-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="bf8d1-106">Herstellen einer Verbindung mit der SPO-PowerShell mit mehrstufiger Authentifizierung (MFA)</span><span class="sxs-lookup"><span data-stu-id="bf8d1-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="bf8d1-107">[SharePoint Patterns and Practices (PNP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) enthält eine Bibliothek mit PowerShell-Befehlen, mit der Sie komplexe Verwaltungsaktionen in Richtung SPO durchführen können.</span><span class="sxs-lookup"><span data-stu-id="bf8d1-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="bf8d1-108">Wenn Sie Probleme beim Herstellen einer Verbindung mit der SPO-Verwaltungsshell haben, stellen Sie sicher, dass Sie die neueste Version aktualisiert haben, und versuchen Sie, [das Modul](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) mit *"Import-Module Microsoft. online. SharePoint. PowerShell"* erneut zu importieren.</span><span class="sxs-lookup"><span data-stu-id="bf8d1-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="bf8d1-109">Wenn Sie versuchen, clientseitige Objektmodell Skripts auszuführen, müssen Sie das [SharePoint Online-Clientkomponenten-SDK](https://www.microsoft.com/download/details.aspx?id=42038) auf Ihrem lokalen Computer installiert haben.</span><span class="sxs-lookup"><span data-stu-id="bf8d1-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="bf8d1-110">Wenn bei der Ausführung von Skripts aus PowerShell Probleme auftreten, können Sie die Ausführung von PowerShell als Administrator und das Ändern der [Ausführungsrichtlinie](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)in Frage stellen.</span><span class="sxs-lookup"><span data-stu-id="bf8d1-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>