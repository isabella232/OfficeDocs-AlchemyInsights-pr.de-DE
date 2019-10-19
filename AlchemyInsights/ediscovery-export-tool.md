---
title: eDiscovery-Export Tool
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/3/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 5a54344d43d16c77d440768aa1c87489edf10ca0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36736324"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Kann das eDiscovery-Export Tool nicht installiert oder ausgeführt werden?

Wenn Sie das Office 365 eDiscovery-Export Tool zum Herunterladen von Suchergebnissen nicht installieren oder ausführen können, überprüfen Sie die folgenden Punkte:
  
- Der verwendete Computer erfüllt die folgenden Voraussetzungen:

  - 32- oder 64-Bit-Versionen von Windows 7 und höher

  - Microsoft .NET Framework 4,7

  - Einen unterstützten Browser:

  - Microsoft Edge

    Oder

  - Internet Explorer 10 und höher

    Andere Browser wie Google Chrome und Mozilla Firefox werden nicht unterstützt.

- Ihre Organisation kann eine Verbindung mit dem Endpunkt in Azure herstellen, also ** \*. BLOB.Core.Windows.net** (der Platzhalter stellt einen eindeutigen Bezeichner für den Exportauftrag dar).

- Sie haben die Rolle Export im Office 365 Security &amp; Compliance Center zugewiesen. Diese Rolle wird standardmäßig nur der Rollengruppe "eDiscovery-Manager" zugewiesen. Weitere Informationen finden Sie unter [Zuweisen von eDiscovery-Berechtigungen](https://docs.microsoft.com/office365/securitycompliance/assign-ediscovery-permissions).

Weitere Informationen finden Sie unter [Exportieren von Inhalts Suchergebnissen](https://docs.microsoft.com/office365/securitycompliance/export-search-results).
  