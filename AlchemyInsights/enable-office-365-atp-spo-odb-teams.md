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
ms.openlocfilehash: 61ca448ef146f3f6fb930f0dc6f09f41bde72087f56ffba820f0a2d517cddb31
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53964632"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivieren von Microsoft Defender für Office 365 für SharePoint Online, OneDrive und Microsoft Teams

1. Wechseln Sie zu https://protection.office.com, und melden Sie sich an.
2. Wählen Sie Die Richtlinie für **die Bedrohungsverwaltung**  >    >  **Tresor Anlagen aus.**
3. Wählen Sie **"Defender für Office 365 für SharePoint, OneDrive und Microsoft Teams** aktivieren" aus, und klicken Sie dann auf **"Speichern".**
4. (Empfohlen) Führen Sie als globaler Administrator oder SharePoint Onlineadministrator das Cmdlet ["Set-SPOTenant"](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) aus, wobei der Parameter **DisallowInfectedFileDownload** auf *"true"* festgelegt ist.
5. (Empfohlen) [Richten Sie Warnungen](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) für erkannte Dateien ein.

> [!NOTE]
> Microsoft Defender für Office 365 überprüft nicht jede einzelne Datei in SharePoint Online, OneDrive oder Microsoft Teams. Dateien werden asynchron durch einen Prozess gescannt, der Freigabe- und Gastaktivitätsereignisse sowie intelligente Heuristiken und Bedrohungssignale verwendet, um schädliche Dateien zu identifizieren. Informationen [zu SharePoint, OneDrive und Microsoft Teams finden Sie unter Microsoft Defender für Office 365.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)