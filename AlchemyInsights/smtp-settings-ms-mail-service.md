---
title: SMTP-Einstellungen für den Microsoft 365-E-Mail-Dienst
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12073"
- "3000003"
ms.openlocfilehash: 261695a0bf736a51514df50c0ad66aaab5b50edb
ms.sourcegitcommit: e9fcd72e64d35f5ba14dfa0fbde39eae20d86cfe
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/27/2021
ms.locfileid: "53603261"
---
# <a name="smtp-settings-for-the-microsoft-365-mail-service"></a>SMTP-Einstellungen für den Microsoft 365-E-Mail-Dienst

Dies sind die SMTP-Einstellungen für die Microsoft 365-E-Mail-Dienste:

**Server**: smtp.office365.com </br>
**Port**: 587 </br>
**Verschlüsselung**: STARTTLS (nur TLS 1.2-Version wird jetzt unterstützt. Stellen Sie sicher, dass Ihre Anwendung oder Ihr Gerät TLS 1.2 unterstützt.) </br>
**Benutzername**: Ihre Office 365-E-Mail-Adresse (z. B. example@yourdomain.com) </br>
**Kennwort**: Ihr Office 365-Kennwort </br>
**Authentifizierung**: Erforderlich </br>
**Sendegrenzwerte**: 10.000 E-Mails pro Tag </br>

Informationen zu POP- und IMAP-Einstellungen finden Sie unter [POP-, IMAP- und SMTP-Einstellungen](https://support.microsoft.com/office/pop-imap-and-smtp-settings-8361e398-8af4-4e97-b147-6c6c4ac95353).
 
Informationen zu den verfügbaren Optionen zum Weiterleiten von E-Mails mithilfe von Microsoft 365 und den Schritten finden Sie unter [Einrichten eines Multifunktionsgeräts oder einer Anwendung zum Senden von E-Mails mithilfe von Microsoft 365 oder Office 365](/exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).