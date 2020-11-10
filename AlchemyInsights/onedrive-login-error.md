---
title: OneDrive-Anmeldefehler AADSTS50011
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
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947501"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive-Anmeldefehler AADSTS50011

Wenn die Fehlermeldung "AADSTS50011: die in der Anforderung angegebene Antwort-URL nicht mit der Antwort übereinstimmt" beim Anmelden bei der OneDrive-App angezeigt wird, überprüfen Sie Folgendes:

Ihre OneDrive-Version muss größer oder gleich der Version 20.052. xxxx sein. XXXX. Um Ihre Version zu überprüfen, klicken Sie auf das blaue OneDrive-Symbol im Infobereich, wählen Sie **Hilfe & Einstellungen > Einstellungen > über** aus.

Ihr Netzwerk blockiert möglicherweise den Datenverkehr zu **g.Live.com** und **oneclient.sfx.ms**. Wenn dieser Datenverkehr blockiert ist, kann OneDrive sich selbst nicht aktualisieren. Arbeiten Sie mit Ihrem Netzwerkadministrator zusammen, um sicherzustellen, dass Sie Zugriff auf diese URLs haben. [Diese Endpunkte](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) sollten für Kunden mit Microsoft 365-Plänen erreichbar sein.

Wenn Sie eine aktuelle Version von OneDrive manuell abrufen möchten, besuchen Sie [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
