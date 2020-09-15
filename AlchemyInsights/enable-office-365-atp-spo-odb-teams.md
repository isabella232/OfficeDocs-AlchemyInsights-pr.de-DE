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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709906"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="34cb4-102">Aktivieren von Office 365 Advanced Threat Protection für SharePoint Online, OneDrive und Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="34cb4-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="34cb4-103">Gehen Sie auf https://protection.office.com, und melden Sie sich an.</span><span class="sxs-lookup"><span data-stu-id="34cb4-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="34cb4-104">Wählen Sie **Threat Management**  >  **Policy**  >  **Safe Attachments**aus.</span><span class="sxs-lookup"><span data-stu-id="34cb4-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="34cb4-105">Wählen Sie **ATP für SharePoint, OneDrive und Microsoft Teams aktivieren**aus, und klicken Sie dann auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="34cb4-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="34cb4-106">Empfohlen Führen Sie als globaler Administrator oder SharePoint Online Administrator das Cmdlet " [SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) " aus, wobei der Parameter " **DisallowInfectedFileDownload** " auf " *true*" festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="34cb4-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="34cb4-107">Empfohlen [Einrichten von Benachrichtigungen](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) für erkannte Dateien.</span><span class="sxs-lookup"><span data-stu-id="34cb4-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="34cb4-108">ATP wird nicht jede einzelne Datei in SharePoint Online, OneDrive oder Microsoft Teams scannen.</span><span class="sxs-lookup"><span data-stu-id="34cb4-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="34cb4-109">Dateien werden asynchron durch einen Prozess überprüft, der Freigabe-und Gast Aktivitätsereignisse verwendet, zusammen mit intelligenten Heuristiken und Bedrohungs Signalen, um bösartige Dateien zu identifizieren.</span><span class="sxs-lookup"><span data-stu-id="34cb4-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="34cb4-110">Siehe [ATP für SharePoint, OneDrive und Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="34cb4-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>