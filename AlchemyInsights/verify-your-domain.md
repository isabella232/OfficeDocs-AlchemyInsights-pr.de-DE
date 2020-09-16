---
title: Verify your domain
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
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734305"
---
# <a name="verify-your-domain"></a>Verify your domain

 **Der Datensatz wurde möglicherweise nicht über das Internet aktualisiert.**
  
In der Regel dauert es nur ein paar Minuten, bis wir den neuen Eintrag sehen können, aber gelegentlich kann es auch ein paar Stunden dauern. 
  
- Wenn Sie schon so lange gewartet haben, überprüfen Sie, ob Sie den exakten Wert kopiert und in den txt-Überprüfungs Eintrag auf Ihrem DNS-Host eingefügt haben. Ein häufiges Problem ist, dass der Teil "MS=" des Eintrags fehlt. Diese Angabe ist ebenfalls erforderlich!

- Bei einigen DNS-Hosts müssen Sie einen zusätzlichen Schritt ausführen, um die Zonendatei zu speichern (in der der DNS-Eintrag gespeichert ist), damit der Eintrag im Internet aktualisiert wird. Stellen Sie sicher, dass Sie Ihre Änderungen gespeichert haben, damit Microsoft den Datensatz sehen und überprüfen kann.
