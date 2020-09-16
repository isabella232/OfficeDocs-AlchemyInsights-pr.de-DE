---
title: Leistungsprobleme – SharePoint oder OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771243"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint oder OneDrive langsam, unzugänglich oder nicht verfügbar für mehrere Benutzer

Wenn eine OneDrive-oder SharePoint-Website nicht für mehrere Benutzer verfügbar ist, die zuvor Zugriff hatten, ist möglicherweise ein vorübergehendes Dienst Problem aufgetreten. [Überprüfen Sie das Dienst Integritäts Dashboard](https://portal.office.com/adminportal/home#/servicehealth).

**Hinzufügen und lizenzieren des Benutzers**

Stellen Sie sicher, dass Sie [Benutzern in Microsoft 365 for Business Lizenzen zuweisen](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**Zuweisen von Berechtigungen**

Wenn dem Benutzer eine SharePoint-Lizenz zugewiesen wurde und weiterhin eine Nachricht mit Zugriff verweigert erhalten wird, stellen Sie sicher, dass Ihnen die [entsprechende Berechtigungsstufe](https://docs.microsoft.com/sharepoint/understanding-permission-levels) zugewiesen ist.

**Verwenden der Access-Anforderungsfunktion in Frage stellen**

Mit der [Zugriffs Anforderungsfunktion](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) können Benutzer Zugriff auf Inhalte anfordern, für die Sie derzeit keine Berechtigung haben.

**Benutzerdefiniertes Skript zulassen verursacht möglicherweise Zugriffs Verweigerungs Probleme**

Es gibt bestimmte Szenarien, in denen das Feature *benutzerdefiniertes Skript zulassen* möglicherweise einen Zugriff verweigert darstellt. Eine Liste der betroffenen Features, Sicherheitsüberlegungen und die Möglichkeit, das Feature zu deaktivieren. Weitere Informationen finden Sie unter [zulassen oder verhindern von benutzerdefiniertem Skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

