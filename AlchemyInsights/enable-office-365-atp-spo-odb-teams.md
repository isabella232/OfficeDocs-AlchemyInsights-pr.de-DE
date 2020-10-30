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
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="0ba30-102">Aktivieren von Microsoft Defender für Office 365 für SharePoint Online, OneDrive und Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="0ba30-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="0ba30-103">Gehen Sie auf https://protection.office.com, und melden Sie sich an.</span><span class="sxs-lookup"><span data-stu-id="0ba30-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="0ba30-104">Wählen Sie **Threat Management**  >  **Policy**  >  **Safe Attachments** aus.</span><span class="sxs-lookup"><span data-stu-id="0ba30-104">Choose **Threat management** > **Policy** > **Safe Attachments** .</span></span>
3. <span data-ttu-id="0ba30-105">Wählen Sie **ATP für SharePoint, OneDrive und Microsoft Teams aktivieren** aus, und klicken Sie dann auf **Speichern** .</span><span class="sxs-lookup"><span data-stu-id="0ba30-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams** , and then click **Save** .</span></span>
4. <span data-ttu-id="0ba30-106">Empfohlen Führen Sie als globaler Administrator oder SharePoint Online Administrator das Cmdlet " [SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) " aus, wobei der Parameter " **DisallowInfectedFileDownload** " auf " *true* " festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="0ba30-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true* .</span></span>
5. <span data-ttu-id="0ba30-107">Empfohlen [Einrichten von Benachrichtigungen](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) für erkannte Dateien.</span><span class="sxs-lookup"><span data-stu-id="0ba30-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="0ba30-108">ATP wird nicht jede einzelne Datei in SharePoint Online, OneDrive oder Microsoft Teams scannen.</span><span class="sxs-lookup"><span data-stu-id="0ba30-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="0ba30-109">Dateien werden asynchron durch einen Prozess überprüft, der Freigabe-und Gast Aktivitätsereignisse verwendet, zusammen mit intelligenten Heuristiken und Bedrohungs Signalen, um bösartige Dateien zu identifizieren.</span><span class="sxs-lookup"><span data-stu-id="0ba30-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="0ba30-110">Siehe [ATP für SharePoint, OneDrive und Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="0ba30-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>