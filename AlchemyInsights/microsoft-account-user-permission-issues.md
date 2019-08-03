---
title: Problembehandlung – Benutzer wurde nicht im Verzeichnis gefunden
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0909edc581c811fdc4683b004e0df0adbac88d1c
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/26/2019
ms.locfileid: "35249912"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Problembehandlung – Benutzer wurde nicht im Verzeichnis gefunden

Wenn Benutzer Fehlermeldung "Benutzer kann nicht gefunden werden" im Verzeichnis empfangen. Versuchen Sie es erneut, wobei der Problemtyp Benutzer nicht im Verzeichnis ist.

Die folgenden Schritte können zur Behandlung des Problems ausgeführt werden.

- Stellen Sie sicher, dass das Konto, mit dem die e-Mail-Einladung angenommen wurde, das gleiche Konto ist, mit dem Sie sich später anmelden. Stellen Sie sicher, dass der Benutzer dasselbe Konto verwendet, um die Einladung zu akzeptieren und sich bei der Website anzumelden. 

Weitere Informationen finden Sie unter [Vorgehensweise Verwalten von Aliasen für</a> Ihr Microsoft-Konto zum Verwalten der Office 365 Anmeldung](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Wechseln Sie zu jedem Standort (en), in dem der Benutzer den Fehler empfängt. 

Fügen Sie "/_layouts/15/people.aspx/membershipgroupid = 0" (innerhalb der Anführungszeichen) am Ende der Website-URL hinzu. 

Beispiel: https://#a0 "Contoso" #a1. SharePoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Wählen Sie den Benutzer aus der Liste aus.

- Klicken Sie im Menüband auf **Benutzerberechtigungen entfernen** . 
-  Fügen Sie den Benutzer wieder hinzu, und senden Sie die Einladung erneut an den Benutzer.

