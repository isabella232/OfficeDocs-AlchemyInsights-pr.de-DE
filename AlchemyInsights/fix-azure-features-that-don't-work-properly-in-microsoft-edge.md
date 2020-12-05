---
title: Vorgehensweise, wenn Azure-Funktionen in Microsoft Edge nicht ordnungsgemäß funktionieren
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576485"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Vorgehensweise, wenn Azure-Funktionen in Microsoft Edge nicht ordnungsgemäß funktionieren

Microsoft Edge hat [bekannte Probleme](https://go.microsoft.com/fwlink/?linkid=2140608) im Zusammenhang mit Sicherheitszonen und wirkt sich möglicherweise darauf aus, wie Azure-Benutzer sich bei Windows Admin Center anmelden. Wenn Sie bei der Verwendung von Azure-Funktionen mit Microsoft Edge Probleme haben, führen Sie die folgenden Schritte aus:

1. Suchen Sie im **Startmenü** nach **Internet Optionen** , und wählen Sie es aus.
2. Wechseln Sie im Dialogfeld **Internet Eigenschaften** zur Registerkarte **Sicherheit** .
3. Wählen Sie die Zone **Vertrauenswürdige Sites** aus, und wählen Sie dann die Schaltfläche **Sites** aus.
4. Fügen Sie im Dialogfeld **vertrauenswürdige Websites** die Gateway-URL sowie [https://login.microsoftonline.com](https://login.microsoftonline.com) und ein [https://login.live.com](https://login.live.com) , und wählen Sie dann **Schließen** aus.
5. Wechseln Sie im Dialogfeld **Internet Eigenschaften** zur Registerkarte **Datenschutz** .
6. Wählen Sie im Abschnitt **Popupblocker** die Option **Einstellungen** aus. Fügen Sie im daraufhin geöffneten Dialogfeld die Gateway-URL sowie und ein [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) , und wählen Sie dann **Schließen** aus.
