---
title: Workflow-e-Mail wird nicht gesendet
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270671"
---
# <a name="workflow-email-is-not-being-sent"></a>Workflow-e-Mail wird nicht gesendet

1. E-Mails aus Workflows werden nicht an alle Benutzer oder nur bestimmte Benutzer gesendet, oder es wird der Fehler angezeigt, dass **die e-Mail-Nachricht nicht gesendet werden kann. Stellen Sie sicher, dass die e-Mail über einen gültigen Empfänger verfügt**.

    Überprüfen Sie, ob der Benutzer in der Gruppe **alle Personen** Berechtigungen (Benutzerinformationsliste) für diese Websitesammlung vorhanden ist.  Beispiel für eine direkte URL<tenant>: https://<sitename>. SharePoint.com/Sites//_layouts/15/people.aspx? MembershipGroupId = 0

    - Wenn der Benutzer nicht vorhanden ist, stellen Sie sicher, dass der Benutzer bei der Seite angemeldet ist. 
    - Wenn es sich um einen externen Benutzer handelt, stellen Sie sicher, dass Ihre Einladung akzeptiert wurde.
    - Wenn der Benutzer in der Gruppe Berechtigungen vorhanden ist, stellen Sie sicher, dass die e-Mail-Adresse richtig ist.
    - Wenn die e-Mail-Adresse des Benutzers hier nicht festgelegt ist, erstellen Sie eine Beispielwarnung für diesen Benutzer, die die Synchronisierung dieses Benutzerkontos von Benutzerprofilen von SharePoint zu dieser Websitesammlung erzwingt.
 
2. E-Mails aus Workflows werden an die Websitesammlungsadministratoren, jedoch nicht an andere Benutzer gesendet, und es wird der Fehler " **http verboten <spam> <spam> ** <spam> <spam>" angezeigt.
 

    Siehe [Zugriff verweigert, wenn e-Mails an Gruppen gesendet werden](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).

    Stellen Sie außerdem sicher, dass das Feature für die **Sperrung der Benutzerberechtigungen für den begrenzten Zugriff** nicht aktiv ist.


## <a name="related-topics"></a>Verwandte Themen
Möchten Sie Microsoft Flow in SharePoint Online testen?
- [Fluss erstellen](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint und Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


