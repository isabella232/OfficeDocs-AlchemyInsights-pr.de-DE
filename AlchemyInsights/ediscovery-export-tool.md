---
title: eDiscovery-Exporttool
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814587"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Kann das eDiscovery-Exporttool nicht installiert oder ausgeführt werden?

Wenn Sie das eDiscovery-Exporttool nicht installieren oder ausführen können, um Suchergebnisse herunterzuladen, überprüfen Sie folgendes:
  
- Der computer, den Sie verwenden, erfüllt die folgenden Voraussetzungen:

  - 32- oder 64-Bit-Versionen von Windows 7 und höher

  - Microsoft .NET Framework 4.7

  - Einen unterstützten Browser:

  - Microsoft Edge

    Oder

  - Internet Explorer 10 und höher

    Andere Browser wie Google Chrome und Mozilla Firefox werden nicht unterstützt.

- Ihre Organisation kann eine Verbindung mit dem Endpunkt in Azure herstellen, der **\* .blob.core.windows.net** ist (der Platzhalter stellt einen eindeutigen Bezeichner für Ihren Exportauftrag dar).

- Ihnen wird die Rolle Export im Microsoft 365 Security &amp; Compliance Center zugewiesen. Diese Rolle wird standardmäßig nur der Rollengruppe eDiscovery Manager zugewiesen. Weitere [Informationen finden Sie unter Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Weitere Informationen finden Sie unter [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Wenn Sie mehr als 100.000-Postfächer exportieren, müssen Sie die folgenden Powershell verwenden, um die Exportergebnisse herunterzuladen: Exportieren von Ergebnissen aus mehr als  [100-K-Postfächern](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).