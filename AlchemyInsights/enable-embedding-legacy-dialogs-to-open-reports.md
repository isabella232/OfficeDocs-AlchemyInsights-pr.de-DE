---
title: Aktivieren der Einbettung von alten Dialogen zum Öffnen von Berichten
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: 285933e607ac7e58256709f0c9cf2851250ce211
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806434"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Aktivieren der Einbettung von alten Dialogen zum Öffnen von Berichten

**Symptom**

Benutzer können keine Berichte öffnen. "Es ist ein Fehler aufgetreten. Überprüfen Sie die technischen Details, um weitere Informationen zu erhalten."

**Ursache**

Berichte können nicht in UCI geladen werden, und der Fehler "Formularbeschreibung ist "null" oder nicht definiert" wird angezeigt. Berichte in UCI erfordern immer noch alte Dialoge, daher muss im System des Kunden *allowlegacydialogsembedding* aktiviert sein.

**Lösung**

1. Navigieren Sie zu **Einstellungen > Verwaltung > Systemeinstellungen > Registerkarte "Allgemein"**.

2. Legen Sie "Einbettung bestimmter alter Dialoge in den Browserclient der einheitlichen Oberfläche aktivieren" auf **Ja** fest.
