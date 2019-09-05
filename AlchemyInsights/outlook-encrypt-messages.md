---
title: S/MIME in Outlook im Internet
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6915470655b85922f6f97e8ca6fac353224b1ae0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752859"
---
# <a name="encrypt-email-messages-in-outlook"></a>E-Mail-Nachrichten in Outlook verschlüsseln

Office 365 Nachrichtenverschlüsselung basiert auf Microsoft Azure Rights Management (Azure RMS), das Teil von Azure Information Protection ist. Wenn Ihr Abonnement Azure Rights Management oder Azure Information Protection umfasst, **müssen Sie keine Aktionen durchführen, um den Rights Management-Dienst manuell zu aktivieren oder zu aktivieren** .

Basierend auf Kundenfeedback können wir Exchange-Nachrichtenfluss Regeln nicht mehr automatisch zum automatischen Verschlüsseln von ausgehenden e-Mails mit bestimmten Typen vertraulicher Informationen in Ihrem Mandanten standardmäßig aktivieren. Stattdessen stellen wir detaillierte Anweisungen dazu bereit, wie Sie dies selbst tun können. Weitere Informationen zum Erstellen einer Transportregel zum Verschlüsseln von vertraulichen Informationen finden Sie in [diesem Artikel](https://aka.ms/OmeEtr).

- Bei Verwendung von Outlook im Internet (ehemals **OWA**): Klicken Sie beim Verfassen einer e-Mail-Nachricht einfach auf in OWA **schützen** . Dies gilt für die Berechtigung "nicht weiterleiten". Klicken Sie auf **Berechtigung ändern** , und wählen Sie **verschlüsseln** , um die Nachricht zu verschlüsseln.

- Wenn Sie **Outlook-Client**verwenden: zum Senden einer verschlüsselten Nachricht von Outlook 2013 oder 2016 oder Outlook 2016 für Mac wählen Sie **options** > **Berechtigungen**aus, und wählen Sie dann die benötigte Schutzoption aus.

- Wenn Sie alle e-Mails, die an bestimmte Empfänger oder externe Partnerorganisationen gesendet werden, **automatisch verschlüsseln** möchten, müssen Sie im Exchange Admin Center eine Nachrichtenfluss-Transportregel erstellen. Ausführliche Anweisungen hierzu finden Sie in [diesem Support-Artikel](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

