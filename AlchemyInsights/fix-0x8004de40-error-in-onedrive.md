---
title: Beheben 0x8004de40 Fehlers in OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649747"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Beheben 0x8004de40 Fehlers in OneDrive

Wenn Sie Windows 7 ausführen und diesen Fehler erhalten, aktualisieren Sie, um [TLS 1.1 und TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)als sichere Standardprotokolle in WinHTTP in Windows zu aktivieren.

Wenn Sie Windows 10 ausführen und eine fehlermeldung 0x8004de40 OneDrive erhalten:

- Starten Sie den betroffenen Computer neu, während er mit Ihrer Acitve Directory-Domäne verbunden ist.
- Wenn das Problem durch einen Neustart nicht behoben werden kann, müssen Sie dieJoinierung ihres Geräts von Azure AD aus wieder auf- und wieder durchführen. 

**Hinweis:** Sie sollten sich in Ihrem Unternehmensnetzwerk befinden, während Sie diese Schritte ausführen. Führen Sie diese Schritte nicht aus, wenn Sie nicht mit Ihrer Unternehmensinfrastruktur verbunden sind (z. B. unterwegs). 

1. Öffnen Sie eine Eingabeaufforderung mit erhöhten Rechten, indem Sie **Start** auswählen, klicken Sie mit der rechten Maustaste auf Eingabeaufforderung, und wählen Sie dann Als Administrator ausführen **aus.**

1. Geben *Sie dsregcmd /leave ein, und* drücken Sie die **EINGABETASTE.**

1. Geben Sie nach Abschluss *des Vorgangs dsregcmd /join ein, und drücken* Sie die **EINGABETASTE.**

1. Schließen Sie nach Abschluss der Eingabeaufforderung die Eingabeaufforderung.

1. Starten Sie den Computer neu, und melden Sie sich bei OneDrive an.