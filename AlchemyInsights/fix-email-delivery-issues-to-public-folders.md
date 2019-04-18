---
title: Beheben von e-Mail-Übermittlungsproblemen für e-Mail-aktivierte Öffentliche Ordner
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: d1c1d5bcb52ba9083e8dd7603feb72436c5154c8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/17/2019
ms.locfileid: "31910597"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Beheben von e-Mail-Übermittlungsproblemen für e-Mail-aktivierte Öffentliche Ordner

Wenn externe Absender keine Nachrichten an Ihre e-Mail-aktivierten Öffentlichen Ordner senden können und die Absender den Fehler erhalten: wurde **nicht gefunden (550 5.4.1)**, überprüfen Sie, ob die e-Mail-Domäne für den öffentlichen Ordner als interne Relay-Domäne anstelle eines autorisierende Domäne:

1. Öffnen Sie das [Exchange Admin Center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Wechseln Sie zu **akzeptierte Domänen**für den **Nachrichtenfluss** \> , wählen Sie die akzeptierte Domäne aus, und klicken Sie dann auf **Bearbeiten**.

3. Ändern Sie auf der Eigenschaftenseite, die geöffnet wird, wenn der Domänentyp auf **autorisierend**festgelegt ist, den Wert in **Internes Relay** , und klicken Sie dann auf **Speichern**.

Wenn externe Absender die Fehlermeldung erhalten, die **Sie nicht über die Berechtigung verfügen (550 5.7.13)**, führen Sie den folgenden Befehl in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) aus, um die Berechtigungen für anonyme Benutzer im öffentlichen Ordner anzuzeigen:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Beispiel: `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Damit externe Benutzer e-Mails an diesen öffentlichen Ordner senden können, fügen Sie dem Benutzer anonymous das Zugriffsrecht createItems hinzu. Beispiel: `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
