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
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543927"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivieren von Microsoft Defender for Office 365 for SharePoint Online, OneDrive und Microsoft Teams

1. Gehen Sie auf https://protection.office.com, und melden Sie sich an.
2. Wählen **Sie Bedrohungsverwaltungsrichtlinie**  >    >  **Sichere Anlagen aus.**
3. Wählen **Sie Aktivieren von Defender für Office 365 für SharePoint, OneDrive und Microsoft Teams aus,** und klicken Sie dann auf **Speichern**.
4. (Empfohlen) Führen Sie als globaler Administrator oder SharePoint Onlineadministrator das [Cmdlet Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) aus, und der **Parameter DisallowInfectedFileDownload** ist auf *true festgelegt.*
5. (Empfohlen) [Richten Sie Warnungen](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) für erkannte Dateien ein.

> [!NOTE]
> Microsoft Defender for Office 365 scannt nicht jede einzelne Datei in SharePoint Online, OneDrive oder Microsoft Teams. Dateien werden asynchron durch einen Prozess überprüft, der Freigabe- und Gastaktivitätsereignisse sowie intelligente Heuristiken und Bedrohungssignale verwendet, um schädliche Dateien zu identifizieren. Weitere [Informationen zu Office 365, SharePoint, OneDrive und](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)Microsoft Teams finden Sie unter Microsoft Defender for Microsoft Teams .