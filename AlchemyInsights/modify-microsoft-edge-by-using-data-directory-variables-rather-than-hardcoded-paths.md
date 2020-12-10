---
title: Ändern von Microsoft Edge mithilfe von Datenverzeichnis Variablen anstelle von hartcodierten Pfaden
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608844"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>Ändern von Microsoft Edge mithilfe von Datenverzeichnis Variablen anstelle von hartcodierten Pfaden

Wenn Sie beispielsweise in Windows die Profildaten unter den lokalen Anwendungsdaten eines Benutzers anstatt am Standardspeicherort speichern möchten, legen Sie die **UserDataDir** -Richtlinie auf **$ {local_app_data} \Edge\Profile**. 

Weitere Informationen finden Sie unter [Create Microsoft Edge User Data Directory variables](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).