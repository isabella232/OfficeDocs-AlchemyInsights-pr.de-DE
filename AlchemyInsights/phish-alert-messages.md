---
title: 2491 Benachrichtigungs-e-Mails von der Richtlinie zum Überschreiben von Phishing-Angriffen durch Mandanten oder Benutzer
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391276"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Benachrichtigung über e-Mail-Nachrichten von der Richtlinie zum Überschreiben von Phishing-Angriffen durch Mandanten oder Benutzer

Für Mandanten mit Office 365 ATP P1-und P2-Lizenzen wurde eine standardmäßige Warnungs Richtlinie mit dem Namen "Phishing, die aufgrund einer Mandanten-oder Benutzer Überschreibung" gesendet wurde, eingeführt. Wenn Sie diese Warnung erhalten haben, führen Sie die folgenden Schritte aus, um Folgendes zu untersuchen:

1. Klicken Sie in der Warnmeldung auf **Warnung anzeigen** , um zur Seite **Benachrichtigungen** im Security #a0 Compliance Center zu wechseln.

2. Wählen Sie die Warnung aus, um die Option zum **Anzeigen der Nachrichtenliste** oder zum **Anzeigen von Nachrichten im Explorer**anzuzeigen. Beide Optionen führen Sie zu den Details der Nachricht, die die Nachrichten-ID enthält. Beachten Sie, dass der Link Threat Explorer automatisch die Nachrichten filtert, die den Warnungskriterien entsprechen. Möglicherweise müssen Sie den Datumsfilter im Threat Explorer anpassen.

Die Phishing-Nachricht wurde aufgrund einer manuell konfigurierten Außerkraftsetzung zugestellt:

- Ein zulässiger Absender oder eine vom Benutzer festgelegte Domäne.

- Ein zulässiger Absender oder eine vom Administrator festgelegte Domäne in einer Anti-Spam-Richtlinie.

- Eine zugelassene IP-Adresse in einer Verbindungsfilter Richtlinie.

- Eine e-Mail-Fluss Regel (auch als Transportregel bezeichnet), die für das Zulassen von Nachrichten in konfiguriert ist.

Wenn Sie der Meinung sind, dass die Nachricht fälschlicherweise als Phishing gekennzeichnet wurde, verwenden Sie das Outlook [-Berichtsnachrichten-Add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) , um Nachrichtenbeispiele an Microsoft zu übermitteln.
