---
title: SMTP-Einstellungen für den Microsoft 365 E-Mail-Dienst
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
ms.openlocfilehash: 373042e9593faf4eaa486313763beb8e8f48b6e9ea159d1cfb37b9df826384f4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54107152"
---
# <a name="smtp-settings-for-the-microsoft-365-mail-service"></a>SMTP-Einstellungen für den Microsoft 365 E-Mail-Dienst

Dies sind die SMTP-Einstellungen für die Microsoft 365 E-Mail-Dienste:

**Server**: smtp.office365.com </br>
**Port**: 587 </br>
**Verschlüsselung**: STARTTLS (nur TLS 1.2-Version wird jetzt unterstützt. Stellen Sie sicher, dass Ihre Anwendung oder Ihr Gerät TLS 1.2 unterstützt.) </br>
**Benutzername**: Ihre Office 365 E-Mail-Adresse (z. B. example@yourdomain.com) </br>
**Kennwort**: Ihr Office 365-Kennwort </br>
**Authentifizierung**: Erforderlich </br>
**Sendegrenzwerte**: 10.000 E-Mails pro Tag </br>

Informationen zu POP- und IMAP-Einstellungen finden Sie unter [POP-, IMAP- und SMTP-Einstellungen](https://support.microsoft.com/office/pop-imap-and-smtp-settings-8361e398-8af4-4e97-b147-6c6c4ac95353).
 
Informationen zu den verfügbaren Optionen zum Weiterleiten von E-Mails mithilfe von Microsoft 365 und den Schritten finden Sie unter [Einrichten eines Multifunktionsgeräts oder einer Anwendung zum Senden von E-Mails mithilfe von Microsoft 365 oder Office 365](/exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).