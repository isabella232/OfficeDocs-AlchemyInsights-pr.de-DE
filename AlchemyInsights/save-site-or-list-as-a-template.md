---
title: Website oder Liste als Vorlage speichern
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 73a32536995a604c734393c2300b4c9bb507e2b2
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770527"
---
# <a name="save-site-or-list-as-a-template"></a>Website oder Liste als Vorlage speichern

SharePoint-Websitevorlagen sind vorkonfigurierte Definitionen, die einem bestimmten Geschäftszweck dienen. Weitere Informationen finden Sie unter [Verwenden von Vorlagen zum Erstellen unterschiedlicher Arten von SharePoint-Websites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Im folgenden finden Sie einige häufige Probleme/Lösungen zum Speichern einer Website oder Liste als Vorlage in SharePoint Online.

**Die Schaltfläche Website/Listenvorlage speichern ist nicht verfügbar oder fehlt**. 

- Administratoren müssen benutzerdefiniertes Skript zulassen, um die Vorlagen Features zu aktivieren. Ausführliche Schritte, Beispiele und Überlegungen finden Sie unter [zulassen oder verhindern von benutzerdefiniertem Skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Der Befehl Website als Vorlage speichern wird nicht unterstützt und kann Probleme auf Websites mit der SharePoint Server Veröffentlichungs Infrastruktur verursachen.


**Die Websitevorlage kann nicht erstellt werden oder funktioniert nicht ordnungsgemäß.**

- Die Vorlage fehlt möglicherweise ein [Feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) und wird nicht aktiviert. Wenn das Feature nicht zur Aktivierung in der aktuellen Websitesammlung verfügbar ist, können Sie die Websitevorlage nicht zum Erstellen einer Website verwenden.


- Überprüfen Sie, ob Listen oder Bibliotheken den Grenzwert für die [Listenansicht](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) von 5000 Elementen überschreiten, da dadurch das Erstellen einer Websitevorlage blockiert werden kann.


- Die Website verwendet möglicherweise zu viele Ressourcen, und daher überschreitet die Websitevorlage den Grenzwert von 50 MB.


- Es gibt Probleme beim Anzeigen von Daten aus einer Liste, die eine Nachschlagespalte verwendet. Weitere Informationen finden Sie unter [Template-generated list zeigt keine Daten aus der richtigen Nachschlageliste in SharePoint Online an](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).


Ausführlichere Informationen zu häufig auftretenden Problemen und Lösungen finden Sie unter Referenz, [Erstellen und Verwenden von Websitevorlagen](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

