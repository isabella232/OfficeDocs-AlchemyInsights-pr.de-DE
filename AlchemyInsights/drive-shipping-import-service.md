---
title: Laufwerkversand im Microsoft 365-Importdienst
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/02/2021
ms.locfileid: "52721692"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a>Laufwerkversand im Microsoft 365-Importdienst

Verwenden Sie den Laufwerksversand, indem Sie die PSTs auf eine Festplatte kopieren und die Festplatte dann an Microsoft senden.

So starten Sie die Anfrage:

1. Wählen Sie im Microsoft 365 Compliance Center unter **Informationsgovernance** die Option **Importieren**.

1. Wählen Sie den **Typ des Importauftrags** aus und wählen Sie dann **Weiter**.

1. Wenn Sie die Schritte für diese Importoption sehen möchten, wählen Sie **Festplattenlaufwerke an einen unserer physischen Standorte versenden**.

Hier sind einige Dinge, die Sie beachten sollten:

- Ihnen muss die Rolle für den Postfachimport/-export in Exchange Online zugewiesen sein, um PST-Dateien in Microsoft 365-Postfächer importieren zu können.
Bei PSTs mit mehr als 20 GB kann die Leistung beeinträchtigt werden.

- Nur 2,5-Zoll-Festkörperlaufwerke (SSDs) oder interne 2,5-/3,5-Zoll-SATA II/III-Festplatten werden unterstützt.
Eine Festplatte, die PST-Dateien enthält, muss mit BitLocker verschlüsselt werden.

- Die Kosten für das Importieren von PST-Dateien in Microsoft 365-Postfächer mithilfe des Laufwerkversands betragen 2 USD pro GB an Daten.

Weitere Informationen zur Verwendung der Laufwerkversandmethode für den Import von PST-Dateien finden Sie unter [Verwenden des Laufwerkversands zum Importieren der PST-Dateien Ihrer Organisation](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).