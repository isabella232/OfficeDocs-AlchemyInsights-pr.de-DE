---
title: Erstellen einer Website in SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: a964751e52972875a8794ce311546f5816a36ca6
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34753707"
---
# <a name="create-sharepoint-sites-using-templates"></a>Erstellen von SharePoint-Websites mithilfe von Vorlagen

SharePoint-Websitevorlagen sind vorkonfigurierte Definitionen, die einem bestimmten Geschäftszweck dienen. Weitere Informationen finden Sie unter [Verwenden von Vorlagen zum Erstellen unterschiedlicher Arten von SharePoint-Websites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Im folgenden finden Sie einige häufige Probleme/Lösungen zum Speichern einer Website oder Liste als Vorlage in SharePoint Online. 

**Schaltfläche ' Website/Listenvorlage speichern ' ist nicht verfügbar oder fehlt**

Administratoren müssen benutzerdefiniertes Skript zulassen, um die Vorlagen Features zu aktivieren. Ausführliche Schritte, Beispiele und Überlegungen finden Sie unter 

- [Zulassen oder Blockieren von benutzerdefinierten Skripts](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Der Befehl Website als Vorlage speichern wird nicht unterstützt und kann Probleme auf Websites mit der SharePoint Server Veröffentlichungs Infrastruktur verursachen.

Die Websitevorlage kann nicht erstellt werden oder funktioniert nicht ordnungsgemäß.

Die Vorlage fehlt möglicherweise ein [Feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) und wird nicht aktiviert. Wenn das Feature nicht zur Aktivierung in der aktuellen Websitesammlung verfügbar ist, können Sie die Websitevorlage nicht zum Erstellen einer Website verwenden.

- Überprüfen Sie, ob Listen oder Bibliotheken den Grenzwert für die [Listenansicht](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) von 5000 Elementen überschreiten, da dadurch das Erstellen einer Websitevorlage blockiert werden kann.

- Die Website verwendet möglicherweise zu viele Ressourcen, und daher überschreitet die Websitevorlage den Grenzwert von 50 MB.


- Es gibt Probleme beim Anzeigen von Daten aus einer Liste, die eine Nachschlagespalte verwendet. Weitere Informationen finden Sie unter [Template-generated list zeigt keine Daten aus der richtigen Nachschlageliste in SharePoint Online an](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).

Ausführlichere Informationen zu häufig auftretenden Problemen und Lösungen finden Sie unter [Erstellen und Verwenden von Websitevorlagen](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



