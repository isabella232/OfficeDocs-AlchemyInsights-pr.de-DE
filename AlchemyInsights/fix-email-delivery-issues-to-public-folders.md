---
title: Beheben von Problemen mit der Zustellung von e-Mails an e-Mail-aktivierte Öffentliche Ordner
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 900b6cc2765937ee005c7e7dce5d33bbdf582601
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752667"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Beheben von Problemen mit der Zustellung von e-Mails an e-Mail-aktivierte Öffentliche Ordner

Wenn externe Absender keine Nachrichten an Ihre e-Mail-aktivierten Öffentlichen Ordner senden können und die Absender den Fehler erhalten: **konnte nicht gefunden werden (550 5.4.1)**, überprüfen Sie, ob die e-Mail-Domäne für den öffentlichen Ordner als interne Relay-Domäne konfiguriert ist und nicht als autorisierende Domäne:

1. Öffnen Sie das [Exchange Admin Center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Wechseln Sie zu **akzeptierte Domänen**für den **Nachrichtenfluss** \> , wählen Sie die akzeptierte Domäne aus, und klicken Sie dann auf **Bearbeiten**.

3. Ändern Sie auf der Seite Eigenschaften, die geöffnet wird, wenn der Domänentyp auf **autorisierend**festgelegt ist, den Wert in **Internes Relay** , und klicken Sie dann auf **Speichern**.

Wenn externe Absender den Fehler erhalten, für den **Sie keine Berechtigung haben (550 5.7.13)**, führen Sie den folgenden Befehl in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) aus, um die Berechtigungen für anonyme Benutzer im öffentlichen Ordner anzuzeigen:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Beispiel: `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Um externen Benutzern das Senden von e-Mails an diesen öffentlichen Ordner zu gestatten, fügen Sie dem Benutzer anonym das Zugriffsrecht CreateItems hinzu. Beispiel: `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
