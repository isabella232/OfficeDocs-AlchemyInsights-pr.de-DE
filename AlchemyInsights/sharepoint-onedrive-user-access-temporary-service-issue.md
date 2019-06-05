---
title: Leistungsprobleme – SharePoint oder OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719516"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint oder OneDrive langsam, unzugänglich oder nicht verfügbar für mehrere Benutzer

Wenn eine OneDrive-oder SharePoint-Website nicht für mehrere Benutzer verfügbar ist, die zuvor Zugriff hatten, ist möglicherweise ein vorübergehendes Dienst Problem aufgetreten. [Überprüfen Sie das Dienst Integritäts Dashboard](https://portal.office.com/adminportal/home#/servicehealth).

## <a name="add-and-license-the-user"></a>Hinzufügen und lizenzieren des Benutzers

Stellen Sie sicher, dass Sie [Benutzern in Office 365 für Unternehmen Lizenzen zuweisen](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


## <a name="assign-permissions"></a>Zuweisen von Berechtigungen

Wenn dem Benutzer eine SharePoint-Lizenz zugewiesen wurde und weiterhin eine Nachricht mit Zugriff verweigert erhalten wird, stellen Sie sicher, dass Ihnen die [entsprechende Berechtigungsstufe](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) zugewiesen ist.

## <a name="consider-using-the-access-request-feature"></a>Verwenden der Access-Anforderungsfunktion in Frage stellen

Mit der [Zugriffs Anforderungsfunktion](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) können Benutzer Zugriff auf Inhalte anfordern, für die Sie derzeit keine Berechtigung haben.

## <a name="allow-custom-script-may-cause-access-denied-issues"></a>Benutzerdefiniertes Skript zulassen verursacht möglicherweise Zugriffs Verweigerungs Probleme

Es gibt bestimmte Szenarien, in denen das Feature *benutzerdefiniertes Skript zulassen* möglicherweise einen Zugriff verweigert darstellt. Eine Liste der betroffenen Features, Sicherheitsüberlegungen und die Möglichkeit, das Feature zu deaktivieren. Weitere Informationen finden Sie unter [zulassen oder verhindern von benutzerdefiniertem Skript](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).

