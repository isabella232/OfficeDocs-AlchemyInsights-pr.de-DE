---
title: S/MIME in Outlook im Web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 7184ffd68f56639a8bcb87e9c6cab88388868103
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764871"
---
# <a name="encrypt-email-messages-in-outlook"></a>E-Mail-Nachrichten in Outlook verschlüsseln

Die Microsoft 365-Nachrichtenverschlüsselung basiert auf Microsoft Azure Rights Management (Azure RMS), das Teil von Azure Information Protection ist. Wenn Ihr Abonnement Azure Rights Management oder Azure Information Protection umfasst, **müssen Sie keine Aktionen durchführen, um den Rights Management-Dienst manuell zu aktivieren oder zu aktivieren** .

Basierend auf Kundenfeedback können wir Exchange-Nachrichtenfluss Regeln nicht mehr automatisch zum automatischen Verschlüsseln von ausgehenden e-Mails mit bestimmten Typen vertraulicher Informationen in Ihrem Mandanten standardmäßig aktivieren. Stattdessen stellen wir detaillierte Anweisungen dazu bereit, wie Sie dies selbst tun können. Weitere Informationen zum Erstellen einer Transportregel zum Verschlüsseln von vertraulichen Informationen finden Sie in [diesem Artikel](https://aka.ms/OmeEtr).

- Bei Verwendung von Outlook im Internet (ehemals **OWA**): Klicken Sie beim Verfassen einer e-Mail-Nachricht einfach auf in OWA **schützen** . Dies gilt für die Berechtigung "nicht weiterleiten". Klicken Sie auf **Berechtigung ändern** , und wählen Sie **verschlüsseln** , um die Nachricht zu verschlüsseln.

- Wenn Sie **Outlook-Client**verwenden: zum Senden einer verschlüsselten Nachricht von Outlook 2013 oder 2016 oder Outlook 2016 für Mac wählen Sie **options** > **Berechtigungen**aus, und wählen Sie dann die benötigte Schutzoption aus.

- Wenn Sie alle e-Mails, die an bestimmte Empfänger oder externe Partnerorganisationen gesendet werden, **automatisch verschlüsseln** möchten, müssen Sie im Exchange Admin Center eine Nachrichtenfluss-Transportregel erstellen. Ausführliche Anweisungen hierzu finden Sie in [diesem Support-Artikel](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

