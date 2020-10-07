---
title: Beheben von Problemen mit der Zustellung von e-Mails an e-Mail-aktivierte Öffentliche Ordner
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
- "1956"
- "3500007"
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366463"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Beheben von Problemen mit der Zustellung von e-Mails an e-Mail-aktivierte Öffentliche Ordner

Wenn externe Absender keine Nachrichten an Ihre e-Mail-aktivierten Öffentlichen Ordner senden können und die Absender den Fehler erhalten: **konnte nicht gefunden werden (550 5.4.1)**, überprüfen Sie, ob die e-Mail-Domäne für den öffentlichen Ordner als interne Relay-Domäne anstelle einer autorisierenden Domäne konfiguriert ist:

1. Öffnen Sie das [Exchange Admin Center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Wechseln Sie **Mail flow** zu \> **akzeptierte Domänen**für den Nachrichtenfluss, wählen Sie die akzeptierte Domäne aus, und klicken Sie dann auf **Bearbeiten**.

3. Ändern Sie auf der Seite Eigenschaften, die geöffnet wird, wenn der Domänentyp auf **autorisierend**festgelegt ist, den Wert in **Internes Relay** , und klicken Sie dann auf **Speichern**.

Wenn externe Absender den Fehler erhalten, für den **Sie keine Berechtigung haben (550 5.7.13)**, führen Sie den folgenden Befehl in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) aus, um die Berechtigungen für anonyme Benutzer im öffentlichen Ordner anzuzeigen:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Beispiel: `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Um externen Benutzern das Senden von e-Mails an diesen öffentlichen Ordner zu gestatten, fügen Sie dem Benutzer anonym das Zugriffsrecht CreateItems hinzu. Beispiel: `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
