---
title: Verwenden von Microsoft Edge basierend auf Chromium-Browsern für den Ediscovery-Export
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
- "3473"
- "3100022"
ms.openlocfilehash: 7ee724e5109effce8883be50e360948313c84b34
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834370"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a>Verwenden von Microsoft Edge basierend auf Chromium-Browsern für den Ediscovery-Export

Aufgrund einer kürzlichen Änderung ist für Microsoft Edge-Browser ClickOnce standardmäßig nicht mehr aktiviert. Um das Microsoft 365 eDiscovery Export Tool weiter zu verwenden, müssen Sie entweder Microsoft Internet Explorer verwenden oder ClickOnce Microsoft Edge aktivieren. 

So aktivieren ClickOnce Unterstützung in Microsoft Edge basierend auf Chromium: 
1. Besuchen Sie in Ihrem Microsoft Edge-Browser edge://flags/#edge-click-once.
2. Ändern Sie für die Option „ClickOnce-Unterstützung“ den Wert von **Standard** oder **Deaktiviert** in **Aktiviert**. 
3. Wählen Sie unten im Browserfenster Neu **starten aus.** <br>
 Die Änderung wird nach dem Neustart von Microsoft Edge wirksam. 

Informationen hierzu und Schritte zum Installieren des Exporttools finden Sie unter: [ Exportieren von Inhaltssuchergebnissen](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).