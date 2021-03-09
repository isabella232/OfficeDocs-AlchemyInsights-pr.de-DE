---
title: Behandeln von Problemen bei der MDATP-Installation auf einem Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568623"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Behandeln von Problemen bei der MDATP-Installation auf einem Mac

Wenn bei der manuellen Installation ein Fehler auftritt, wird auf der Seite **Zusammenfassung** des Installations-Assistenten der folgende Fehler angezeigt:

"Bei der Installation ist ein Fehler aufgetreten. Beim Installer ist ein Fehler aufgetreten, der zu einem Fehler bei der Installation führte. Wenden Sie sich an den Softwarehersteller, um Unterstützung zu erhalten."

Bei MDM-Bereitstellungen zeigt die Seite auch einen allgemeinen Installationsfehler an.

Obwohl endbenutzern keine genauen Fehler angezeigt werden, wird eine Protokolldatei mit Dem Installationsfortschritt in **/Library/Logs/Microsoft/mdatp/install.log gespeichert.** Jede Installationssitzung wird an diese Protokolldatei angefügt. Verwenden Sie zum Ausgabe der letzten Installationssitzung `sed` .

Weitere Informationen finden Sie unter [Beheben von Installationsproblemen für Microsoft Defender ATP für Mac](https://go.microsoft.com/fwlink/?linkid=2144615).
