---
title: Wiederherstellen einer gelöschten Microsoft 365-Gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597442"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Wiederherstellen einer gelöschten Microsoft 365-Gruppe

Sie können eine gelöschte Microsoft 365-Gruppe oder Microsoft Teams innerhalb von 30 Tagen nach dem Löschen wiederherstellen.

1. Wechseln Sie zum [Microsoft 365 Admin Center,](https://aka.ms/RestoreDeletedGroup) um sich zu melden und die gelöschten Gruppen und Teams auflisten.

    **Hinweis:** Melden Sie sich mit dem Konto an, das entweder dem Mandantenadministrator oder der Gruppenadministratorrolle zugewiesen ist.

1. Wählen Sie die gelöschte Microsoft 365-Gruppe/Teams aus, die wiederhergestellt werden soll, und klicken Sie auf **Wiederherstellungsgruppe**.

    Wenn die Gruppe aufgrund einer in Konflikt enden SMTP-Adresse nicht wiederhergestellt werden kann, verwenden Sie den folgenden Befehl, um das Objekt zu finden, das einen Konflikt verursacht, und entfernen Sie die SMTP-Adresse:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Hinweis:** In einigen Fällen kann es bis zu 24 Stunden dauern, bis die Gruppe und alle ihre Daten wiederhergestellt werden.

    Weitere Informationen oder Informationen zum Wiederherstellen von Gruppen mithilfe von PowerShell finden Sie unter [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).