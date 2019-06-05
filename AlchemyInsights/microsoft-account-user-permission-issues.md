---
title: Erstellen und Verwenden eines freigegebenen Postfachs
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717346"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Problembehandlung – Benutzer wurde nicht im Verzeichnis gefunden

<p>Wenn Benutzer Fehlermeldungen <strong> &ldquo; &hellip;empfangen,&rsquo;kann der Benutzer im Verzeichnis nicht gefunden werden. Versuchen Sie es&hellip; erneut</strong> , wenn der Problemtyp <strong> &ldquo;Benutzer nicht im Verzeichnis&rdquo;ist.</strong>, die folgenden Schritte können zur Problembehandlung ausgeführt werden.</p> <ol> <li>Stellen Sie sicher, dass das Konto, mit dem die e-Mail-Einladung angenommen wurde, das gleiche Konto ist, mit dem Sie sich später anmelden. Stellen Sie sicher, dass der Benutzer dasselbe Konto verwendet, um die Einladung zu akzeptieren und sich bei der Website anzumelden. <br /><br />Weitere Informationen finden Sie unter <a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">Vorgehensweise Verwalten von Aliasen für Ihr Microsoft-Konto</a> zum Verwalten der Office 365 Anmeldung. <br /><br /></li> <li>Wechseln Sie zu jedem Standort (en), in dem der Benutzer den Fehler empfängt. <br /><br />a. Fügen Sie <strong> &ldquo;/_layouts/15/people.aspx/membershipgroupid =&rdquo; 0</strong> (innerhalb der doppelten Anführungszeichen) am Ende der Website-URL hinzu. <br /><br />Beispiel: https://&lt;Contoso&gt;. SharePoint.com/_layouts/15/people.aspx/membershipGroupId=0 <br /><br />b. Wählen Sie den Benutzer aus der Liste aus. <br /><br />c. Klicken Sie <strong>im Menüband auf Benutzerberechtigungen entfernen</strong>. <br /><br />d. Fügen Sie den Benutzer wieder hinzu, und senden Sie die Einladung erneut an den Benutzer.</li> </ol>

