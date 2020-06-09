---
title: 'Fehler: die Regeln auf diesem Computer stimmen nicht überein'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: ecc1e5ec741cc90c58698991c3a3135f87c39938
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617971"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Fehler: die Regeln auf diesem Computer stimmen nicht überein

Wenn Sie den aktualisierten Status dieses bekannten Problems sehen möchten, lesen Sie [die Regeln auf diesem Computer nicht mit den Regeln für Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Das Outlook-Team hat ein Update in Build 12928,10000 implementiert. Das Update ist bereits bei Insider fast und wird in den monatlichen Kanal Ende Juni 2020 gehen. Sobald Sie den festen Build haben, erhalten Sie möglicherweise die Eingabeaufforderung "welche Regeln möchten Sie beibehalten?" ein letztes Mal. Wählen Sie Server aus, wenn Sie dazu aufgefordert werden, und wechseln Sie dann in Outlook zurück, und aktivieren Sie alle deaktivierten Regeln erneut.

Verwenden Sie die folgende Problemumgehung, bis das Update verfügbar ist:

**Problemumgehung**: in den letzten Berichten ist das Problem bei denjenigen aufgetreten, die nur Clientregeln in Outlook-Desktop erstellt haben. Wenn Sie weiterhin auf das Problem stoßen, sollten Sie die Regeln löschen und dann Regeln nur in OWA (Outlook Web App) erstellen und bearbeiten, bis das Problem behoben ist.

Wenn Sie die Regeln nicht manuell löschen können, können Sie beim Starten von Outlook einen Outlook-Befehl ausführen, indem Sie Outlook. exe/Cleanrules. ausführen. Dadurch werden sowohl die Client-als auch die Server Regeln gelöscht. Dadurch werden alle Regeln für alle Konten im Outlook-Profil gelöscht. Dieser Befehl wird im Artikel Befehlszeilenoptionen weiter beschrieben.