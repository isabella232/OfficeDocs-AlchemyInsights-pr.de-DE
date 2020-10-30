---
title: Aktivieren Office 365 ATP für SharePoint, OneDrive und Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801047"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivieren von Microsoft Defender für Office 365 für SharePoint Online, OneDrive und Microsoft Teams

1. Gehen Sie auf https://protection.office.com, und melden Sie sich an.
2. Wählen Sie **Threat Management**  >  **Policy**  >  **Safe Attachments** aus.
3. Wählen Sie **ATP für SharePoint, OneDrive und Microsoft Teams aktivieren** aus, und klicken Sie dann auf **Speichern** .
4. Empfohlen Führen Sie als globaler Administrator oder SharePoint Online Administrator das Cmdlet " [SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) " aus, wobei der Parameter " **DisallowInfectedFileDownload** " auf " *true* " festgelegt ist.
5. Empfohlen [Einrichten von Benachrichtigungen](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) für erkannte Dateien.

> [!NOTE]
> ATP wird nicht jede einzelne Datei in SharePoint Online, OneDrive oder Microsoft Teams scannen. Dateien werden asynchron durch einen Prozess überprüft, der Freigabe-und Gast Aktivitätsereignisse verwendet, zusammen mit intelligenten Heuristiken und Bedrohungs Signalen, um bösartige Dateien zu identifizieren. Siehe [ATP für SharePoint, OneDrive und Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).