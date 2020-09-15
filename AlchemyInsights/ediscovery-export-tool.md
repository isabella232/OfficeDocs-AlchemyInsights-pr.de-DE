---
title: eDiscovery-Export Tool
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 55f29fae0878917eaf2972ba1dfd3c5b8a26ce54
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711094"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Kann das eDiscovery-Export Tool nicht installiert oder ausgeführt werden?

Wenn Sie das eDiscovery-Export Tool zum Herunterladen von Suchergebnissen nicht installieren oder ausführen können, überprüfen Sie die folgenden Punkte:
  
- Der verwendete Computer erfüllt die folgenden Voraussetzungen:

  - 32- oder 64-Bit-Versionen von Windows 7 und höher

  - Microsoft .NET Framework 4.7

  - Einen unterstützten Browser:

  - Microsoft Edge

    Oder:

  - Internet Explorer 10 und höher

    Andere Browser wie Google Chrome und Mozilla Firefox werden nicht unterstützt.

- Ihre Organisation kann eine Verbindung mit dem Endpunkt in Azure herstellen, also ** \* . BLOB.Core.Windows.net** (der Platzhalter stellt einen eindeutigen Bezeichner für den Exportauftrag dar).

- Sie haben die Rolle Export im Microsoft 365 Security &amp; Compliance Center zugewiesen. Diese Rolle wird standardmäßig nur der Rollengruppe "eDiscovery-Manager" zugewiesen. Weitere Informationen finden Sie unter [Zuweisen von eDiscovery-Berechtigungen](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Weitere Informationen finden Sie unter [Exportieren von Inhalts Suchergebnissen](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).
  