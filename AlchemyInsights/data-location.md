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
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655281"
---
# <a name="data-location"></a>Datenspeicherort

Sie können den Standort Ihres Mandanten im Admin Center anzeigen oder über PowerShell eine Verbindung mit Exchange Online herstellen.


**Admin Center:**
1. Melden Sie sich beim [Admin Center](https://admin.microsoft.com/Adminportal/Home)an.
2. Wählen Sie**Organisationsprofil**für **Einstellungen** > aus.
3. Wählen Sie unter **Datenspeicherort**die Option **Details anzeigen**aus.


**PowerShell**
1. Stellen Sie mithilfe von Windows PowerShell eine Verbindung zu Exchange Online her.
2. Führen Sie das Cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) aus, um eine Liste der Eigenschaften Ihres Mandanten anzuzeigen. 
3. Sehen Sie sich die Organizational-Eigenschaft an.

Wenn Sie den Datenspeicherort für Exo und SPO haben, können Sie den Datenspeicherort für andere Dienste bestimmen, die Sie von der Stelle aus, an der [sich Ihre Daten befinden](https://products.office.com/where-is-your-data-located), verwenden können.