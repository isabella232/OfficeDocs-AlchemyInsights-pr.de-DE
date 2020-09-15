---
title: Erste Schritte mit SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700706"
---
# <a name="workflows-in-sharepoint"></a>Workflows in SharePoint

Wenn SharePoint-Workflows keine e-Mails senden, hat Ihre Organisation möglicherweise die Exchange Online Absender Grenzwerte erkannt.

Die Fehlermeldung "Workflow ist angehalten" kann auftreten, wenn Sie eines der folgenden Elemente haben:

- Sie verfügen über einen Workflow in SharePoint Online, der den SharePoint 2010 oder SharePoint 2013 Workflow-Plattformtyp verwendet.

- Der Workflow ist so konfiguriert, dass eine benutzerdefinierte e-Mail-Nachricht an mehr als 200 Benutzer gleichzeitig gesendet wird, mehr als 10.000 Empfänger pro Tag oder mehr als 30 Nachrichten pro Minute.

Wenn Sie den Workflow ausführen, wird die e-Mail-Nachricht nicht gesendet, und Sie werden feststellen, dass die Fehlermeldung, der interne Status auf angehalten festgelegt oder an einen Empfänger nicht gesendet werden kann, angezeigt wird.

Weitere Informationen finden Sie im folgenden [Artikel](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).

