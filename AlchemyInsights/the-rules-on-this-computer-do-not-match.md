---
title: 'Fehler: Die Regeln auf diesem Computer entsprechen nicht'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782951"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Fehler: Die Regeln auf diesem Computer entsprechen nicht

Informationen zum aktualisierten Status dieses bekannten Problems finden Sie unter Die Regeln auf diesem Computer entsprechen nicht den [Regeln in Microsoft Exchange.](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Das Outlook-Team hat eine Korrektur in Build 12928.10000 implementiert. Der Fix ist bereits bei Insider Fast und wird Ende Juni 2020 zum monatlichen Kanal wechseln. Sobald Sie den festen Build haben, erhalten Sie möglicherweise ein letztes Mal die Eingabeaufforderung "Welche Regeln möchten Sie behalten". Wählen Sie Server, wenn Sie dazu aufgefordert werden, und wechseln Sie dann zurück in Outlook, und aktivieren Sie alle deaktivierten Regeln erneut.

Verwenden Sie die folgende Problemumgehung, bis die Korrektur verfügbar ist:

**Problemumgehung**: In den letzten Berichten ist das Problem für diejenigen aufgetreten, die nur Clientregeln in Outlook Desktop erstellt haben. Wenn das Problem weiterhin besteht, sollten Sie die Regeln löschen und regeln dann nur in OWA (Outlook Web App) erstellen und bearbeiten, bis das Problem behoben ist.

Wenn Sie die Regeln nicht manuell löschen können, können Sie beim Starten von Outlook einen Outlook-Befehl ausführen, indem Sie Outlook.exe /cleanrules ausführen. Dadurch werden sowohl die Client- als auch die Serverregeln gelöscht. Es werden alle Regeln für alle Konten im Outlook-Profil gelöscht. Dieser Befehl wird im Artikel Befehlszeilenschalter weiter dokumentiert.

