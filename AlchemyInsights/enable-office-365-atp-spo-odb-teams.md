---
title: Aktivieren Office 365 ATP für SharePoint, OneDrive und Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703425"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivieren von Office 365 Advanced Threat Protection für SharePoint Online, OneDrive und Microsoft Teams

1. Gehen Sie auf https://protection.office.com, und melden Sie sich an.
2. Wählen Sie **Threat Management** > **Policy** > **Safe Attachments**aus.
3. Wählen Sie **ATP für SharePoint, OneDrive und Microsoft Teams aktivieren**aus, und klicken Sie dann auf **Speichern**.
4. Empfohlen Führen Sie als globaler Administrator oder SharePoint Online Administrator das Cmdlet " [SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) " aus, wobei der Parameter " **DisallowInfectedFileDownload** " auf " *true*" festgelegt ist.
5. Empfohlen [Einrichten von Benachrichtigungen](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) für erkannte Dateien.

> [!NOTE]
> ATP wird nicht jede einzelne Datei in SharePoint Online, OneDrive oder Microsoft Teams scannen. Dateien werden asynchron durch einen Prozess überprüft, der Freigabe-und Gast Aktivitätsereignisse verwendet, zusammen mit intelligenten Heuristiken und Bedrohungs Signalen, um bösartige Dateien zu identifizieren. Weitere Informationen finden Sie unter [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).