---
title: Fix 0x8004de40-Fehler in OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745129"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Fix 0x8004de40-Fehler in OneDrive

Wenn Sie einen 0x8004de40-Fehler mit OneDrive erhalten:

- Starten Sie den betroffenen Computer neu, während eine Verbindung mit ihrer Acitve-Verzeichnisdomäne besteht.
- Wenn das Problem durch einen Neustart nicht behoben werden kann, trennen Sie die Verbindung und fügen Sie Ihr Gerät von Azure AD wieder hinzu. 

**Hinweis**: Wenn Sie diese Schritte ausführen, sollten Sie sich im Unternehmensnetzwerk befinden. Führen Sie diese Schritte nicht aus, wenn Sie nicht in der Lage sind, eine Verbindung mit Ihrer Unternehmensinfrastruktur herzustellen (beispielsweise auf Reisen). 

- Öffnen Sie eine Eingabeaufforderung mit erhöhten Rechten. 
- Klicken Sie zum Öffnen einer Eingabeaufforderung mit erhöhten Rechten auf- **Start**, klicken Sie mit der rechten Maustaste auf **Eingabeaufforderung**, und klicken Sie dann auf **als Administrator ausführen**.
- Geben Sie *dsregcmd/Leave* ein, und drücken **Sie die Eingabe**Taste.
- Geben Sie nach Abschluss *dsregcmd/Join* ein, und drücken **Sie die Eingabe**Taste.
- Schließen Sie nach Abschluss der Eingabeaufforderung.
- Starten Sie den Computer neu, und melden Sie sich bei OneDrive an.