---
title: Datenspeicherort
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207260"
---
# <a name="data-location"></a>Datenspeicherort

Sie können den Speicherort des Office 365 Mandanten im Admin Center anzeigen oder über PowerShell eine Verbindung mit Exchange Online herstellen.


**Admin Center:**
1. Melden Sie sich beim [Admin Center](https://admin.microsoft.com/Adminportal/Home)an.
2. Wählen Sie**Organisationsprofil**für **Einstellungen** > aus.
3. Wählen Sie unter **Datenspeicherort**die Option **Details anzeigen**aus.


**PowerShell**
1. Stellen Sie mithilfe von Windows PowerShell eine Verbindung zu Exchange Online her.
2. Führen Sie das Cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) aus, um eine Liste der Eigenschaften Ihres Mandanten anzuzeigen. 
3. Sehen Sie sich die Organizational-Eigenschaft an.

Wenn Sie den Datenspeicherort für Exo und SPO haben, können Sie den Datenspeicherort für andere Dienste bestimmen, die Sie von der Stelle aus, an der [sich Ihre Daten befinden](https://products.office.com/where-is-your-data-located), verwenden können.