---
title: Fix 0x8004de40-Fehler in OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052036"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Fix 0x8004de40-Fehler in OneDrive

Wenn Sie einen 0x8004de40-Fehler mit OneDrive erhalten:

- Starten Sie den betroffenen Computer neu, während eine Verbindung mit ihrer Acitve-Verzeichnisdomäne besteht.
- Wenn das Problem durch einen Neustart nicht behoben werden kann, trennen Sie die Verbindung und fügen Sie Ihr Gerät von Azure AD wieder hinzu. 

**Hinweis**: Wenn Sie diese Schritte ausführen, sollten Sie sich im Unternehmensnetzwerk befinden. Führen Sie diese Schritte nicht aus, wenn Sie nicht in der Lage sind, eine Verbindung mit Ihrer Unternehmensinfrastruktur herzustellen (beispielsweise auf Reisen). 

- Öffnen Sie die Eingabeaufforderung mit erhöhten Rechten. 
- Klicken Sie zum Öffnen einer Eingabeaufforderung mit erhöhten Rechten auf- **Start**, klicken Sie mit der rechten Maustaste auf **Eingabeaufforderung**, und klicken Sie dann auf **als Administrator ausführen**.
- Geben Sie *dsregcmd/Leave* ein, und drücken **Sie die Eingabe**Taste.
- Geben Sie nach Abschluss *dsregcmd/Join* ein, und drücken **Sie die Eingabe**Taste.
- Schließen Sie nach Abschluss der Eingabeaufforderung.
- Starten Sie den Computer neu, und melden Sie sich bei OneDrive an.