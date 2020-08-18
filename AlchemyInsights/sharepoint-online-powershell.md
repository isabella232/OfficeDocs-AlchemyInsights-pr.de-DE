---
title: SharePoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 300c07e7f0010eae2bd4fe893ece9d09aab93ba5
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786888"
---
# <a name="sharepoint-online-powershell"></a>SharePoint Online PowerShell

Arbeiten mit PowerShell oder Skripts in SharePoint Online? Weitere Informationen finden Sie unter den folgenden Links.
- [Erste Schritte mit der SharePoint Online-Verwaltungsshell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Herstellen einer Verbindung mit der SPO-PowerShell mit mehrstufiger Authentifizierung (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint Patterns and Practices (PNP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) enthält eine Bibliothek mit PowerShell-Befehlen, mit der Sie komplexe Verwaltungsaktionen in Richtung SPO durchführen können.

> [!NOTE]
> - Wenn Sie Probleme beim Herstellen einer Verbindung mit der SPO-Verwaltungsshell haben, stellen Sie sicher, dass Sie die neueste Version aktualisiert haben, und versuchen Sie, [das Modul](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) mit *"Import-Module Microsoft. online. SharePoint. PowerShell"* erneut zu importieren.
> - Wenn Sie versuchen, clientseitige Objektmodell Skripts auszuführen, müssen Sie das [SharePoint Online-Clientkomponenten-SDK](https://www.microsoft.com/download/details.aspx?id=42038) auf Ihrem lokalen Computer installiert haben.
> - Wenn bei der Ausführung von Skripts aus PowerShell Probleme auftreten, können Sie die Ausführung von PowerShell als Administrator und das Ändern der [Ausführungsrichtlinie](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)in Frage stellen.