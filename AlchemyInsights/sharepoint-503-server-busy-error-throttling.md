---
title: Einschränkungen in SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 2aca55ac2fefbb2035140a759a77730dc905a4e9
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958718"
---
# <a name="sharepoint-online-throttling"></a>Einschränkungen in SharePoint Online

**Wichtig**: in diesen noch nie dagewesenen Zeiten werden Maßnahmen ergriffen, um sicherzustellen, dass SharePoint Online-und OneDrive-Dienste hoch verfügbar bleiben – weitere Informationen finden Sie unter [SharePoint Online Anpassungen temporärer Funktionen](https://aka.ms/ODSPAdjustments) .

**503 Server ist besetzt (Fehler)**

Bei dem Versuch, zu SharePoint-oder OneDrive-Websites zu navigieren, erhalten Benutzer möglicherweise einen Fehler "503 Server ist ausgelastet". 

Dieser Fehler kann durch Drosselung im SharePoint-Dienst verursacht werden. SharePoint Online verwendet Einschränkung, um eine optimale Leistung und Zuverlässigkeit des Diensts SharePoint Online verwalten. Einschränkungsgrenzwerte Ruft die Anzahl von Aktionen eines Benutzers oder gleichzeitige (von Code- oder Skriptblock), um Ressourcen zu verhindern. 

Weitere Informationen zur Drosselung finden Sie unter vermeiden Sie eine [Drosselung oder Blockierung in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

Wenn Sie der Meinung sind, dass dieser Fehler nicht mit der Einschränkung zusammenhängt, können Sie überprüfen, ob eine aktive Wartung auf Ihrem Mandanten erfolgt, indem Sie zum [Nachrichtencenter](https://portal.office.com/adminportal/home#/MessageCenter)navigieren.

 Vergewissern Sie sich schließlich, dass Sie die Seite [Dienst Integrität](https://portal.office.com/adminportal/home#/servicehealth) besuchen, um nach eventuell auftretenden Warnungen/Vorfällen zu suchen.

