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
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506917"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="bad90-102">Aktivieren von Office 365 Advanced Threat Protection für SharePoint Online, OneDrive und Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="bad90-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="bad90-103">Gehen Sie auf https://protection.office.com, und melden Sie sich an.</span><span class="sxs-lookup"><span data-stu-id="bad90-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="bad90-104">Wählen Sie **Threat Management**  >  **Policy**  >  **Safe Attachments**aus.</span><span class="sxs-lookup"><span data-stu-id="bad90-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="bad90-105">Wählen Sie **ATP für SharePoint, OneDrive und Microsoft Teams aktivieren**aus, und klicken Sie dann auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="bad90-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="bad90-106">Empfohlen Führen Sie als globaler Administrator oder SharePoint Online Administrator das Cmdlet " [SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) " aus, wobei der Parameter " **DisallowInfectedFileDownload** " auf " *true*" festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="bad90-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="bad90-107">Empfohlen [Einrichten von Benachrichtigungen](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) für erkannte Dateien.</span><span class="sxs-lookup"><span data-stu-id="bad90-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="bad90-108">ATP wird nicht jede einzelne Datei in SharePoint Online, OneDrive oder Microsoft Teams scannen.</span><span class="sxs-lookup"><span data-stu-id="bad90-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="bad90-109">Dateien werden asynchron durch einen Prozess überprüft, der Freigabe-und Gast Aktivitätsereignisse verwendet, zusammen mit intelligenten Heuristiken und Bedrohungs Signalen, um bösartige Dateien zu identifizieren.</span><span class="sxs-lookup"><span data-stu-id="bad90-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="bad90-110">Siehe [ATP für SharePoint, OneDrive und Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="bad90-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>