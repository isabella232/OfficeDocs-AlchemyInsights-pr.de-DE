---
title: E-Mail-Nachrichten in das Archivpostfach migrieren
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799779"
---
# <a name="move-email-to-the-archive-mailbox"></a>E-Mail-Nachricht in das Archivpostfach migrieren

Wenn Sie möchten, dass automatisierte Prüfungen für die unten aufgeführten Einstellungen ausgeführt werden, wählen Sie die Schaltfläche Zurück <--oben auf dieser Seite aus, und geben Sie dann die e-Mail-Adresse des Benutzers ein, der Probleme beim Verschieben von e-Mails in das Archivpostfach hat.

1. Stellen Sie sicher, dass ein **Archivpostfach** aktiviert wurde. Wenn dies nicht der Fall ist, verwenden Sie die Schritte in [diesem Artikel](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) , um das Archivpostfach zu aktivieren.

2. Um Nachrichten automatisch in das Archivpostfach zu archivieren, muss ein Aufbewahrungs mit der Aktion **in Archiv** verlegen auf **automatisch auf gesamtes Postfach (Standard) angewendet**werden. Verwenden Sie die Schritte hier, um das Tag: [Archive default-Tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)zu erstellen.

3. Fügen Sie als nächstes das **Archiv** -Tag zu ihrer Aufbewahrungsrichtlinie hinzu. Wählen Sie in der Exchange-Verwaltungskonsole die Option **Aufbewahrungsrichtlinien** > fügen Sie der Richtlinie > **Speichern**das **Element zum Archivieren** hinzu.

4. [Weisen Sie die Aufbewahrungsrichtlinie](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) nun dem Postfach des jeweiligen Benutzers zu. Dieselbe Richtlinie wird sowohl auf das **primäre** als auch auf das **Archiv** Postfach angewendet.

Es kann erforderlich sein, die Ausführung des Assistenten für verwaltete Ordner (MFA) zu erzwingen und die neuen Einstellungen auf das Postfach des Benutzers anzuwenden. Führen Sie den folgenden Befehl aus, während eine [Verbindung mit Exo PowerShell hergestellt](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) wurde, um den Assistenten für verwaltete Ordner für ein bestimmtes Postfach zu starten:
  
Start-ManagedFolderAssistant-Identity <name of the mailbox>

Weitere Informationen zum Einrichten einer Archivrichtlinie finden Sie unter [Einrichten einer Archiv-und Löschrichtlinie für Postfächer](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  