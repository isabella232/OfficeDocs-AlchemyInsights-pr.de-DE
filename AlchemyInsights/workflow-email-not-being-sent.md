---
title: Workflow-e-Mail wird nicht gesendet
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049372"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Workflow-e-Mails werden nicht für eine SharePoint-Liste oder-Bibliothek gesendet.

1. E-Mails aus Workflows werden nicht an alle Benutzer oder nur bestimmte Benutzer gesendet, oder es wird der Fehler angezeigt, dass **die e-Mail-Nachricht nicht gesendet werden kann. Stellen Sie sicher, dass die e-Mail über einen gültigen Empfänger verfügt**.

    Überprüfen Sie, ob der Benutzer in der Gruppe **alle Personen** Berechtigungen (Benutzerinformationsliste) für diese Websitesammlung vorhanden ist.  Beispiel für eine direkte URL<tenant>: https://<sitename>. SharePoint.com/Sites//_layouts/15/people.aspx? MembershipGroupId = 0

    - Wenn der Benutzer nicht vorhanden ist, stellen Sie sicher, dass der Benutzer bei der Seite angemeldet ist. 
    - Wenn es sich um einen externen Benutzer handelt, stellen Sie sicher, dass Ihre Einladung akzeptiert wurde.
    - Wenn der Benutzer in der Gruppe Berechtigungen vorhanden ist, stellen Sie sicher, dass die e-Mail-Adresse richtig ist.
    - Wenn die e-Mail-Adresse des Benutzers hier nicht festgelegt ist, erstellen Sie eine Beispielwarnung für diesen Benutzer, die die Synchronisierung dieses Benutzerkontos von Benutzerprofilen von SharePoint zu dieser Websitesammlung erzwingt.
 
2. E-Mails aus Workflows werden an die Websitesammlungsadministratoren, jedoch nicht an andere Benutzer gesendet, und es wird der Fehler " **http verboten" für <span>https angezeigt:</span>//URL/_vti_bin/Client.xvc.SP.Utilities.Utility.SendEmail**.
 

    Siehe [Zugriff verweigert, wenn Sie eine e-Mail an eine SharePoint-Gruppe senden](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Stellen Sie außerdem sicher, dass das Feature für die **Sperrung der Benutzerberechtigungen für den begrenzten Zugriff** nicht aktiv ist.


## <a name="related-topics"></a>Verwandte Themen
Möchten Sie Microsoft Flow in SharePoint Online testen?
- [Fluss erstellen](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint und Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


