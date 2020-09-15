---
title: ATP für SharePoint, OneDrive und Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715560"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP für SharePoint, OneDrive und Microsoft Teams

Führen Sie die folgenden Schritte aus, um Advanced Threat Protection zu aktivieren:

1. Wechseln Sie zu, [https://protection.office.com](https://protection.office.com) und melden Sie sich mit einem globalen Administrator-oder Sicherheitsadministrator Konto an.

2. Wählen Sie im linken Navigationsbereich unter **Bedrohungs Verwaltung**die Option **Richtlinien** für \> **sichere Anlagen**aus.

3. Wählen Sie **ATP für SharePoint, OneDrive und Microsoft Teams aktivieren**aus.

4. [Erstellen Sie eine Aktivitäts Warnungs Richtlinie](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) zum Empfangen von Benachrichtigungen, wenn wir bösartige Dateien erkennen.

Ausführliche Anweisungen finden Sie in diesem [Thema](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Hinweis**: ATP scannt nicht jede einzelne Datei in SharePoint Online, OneDrive für Unternehmen oder Microsoft Teams. Dateien werden asynchron durch einen Prozess gescannt, der freigabeaktivitäten, Gast Aktivitäten und Bedrohungs Signale verwendet, um bösartige Dateien zu identifizieren. Weitere Informationen finden Sie in diesem [Thema](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
