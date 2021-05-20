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
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="f60b5-102">Aktivieren von Microsoft Defender for Office 365 for SharePoint Online, OneDrive und Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="f60b5-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="f60b5-103">Gehen Sie auf https://protection.office.com, und melden Sie sich an.</span><span class="sxs-lookup"><span data-stu-id="f60b5-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="f60b5-104">Wählen **Sie Bedrohungsverwaltungsrichtlinie**  >    >  **Sichere Anlagen aus.**</span><span class="sxs-lookup"><span data-stu-id="f60b5-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="f60b5-105">Wählen **Sie Aktivieren von Defender für Office 365 für SharePoint, OneDrive und Microsoft Teams aus,** und klicken Sie dann auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="f60b5-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="f60b5-106">(Empfohlen) Führen Sie als globaler Administrator oder SharePoint Onlineadministrator das [Cmdlet Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) aus, und der **Parameter DisallowInfectedFileDownload** ist auf *true festgelegt.*</span><span class="sxs-lookup"><span data-stu-id="f60b5-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="f60b5-107">(Empfohlen) [Richten Sie Warnungen](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) für erkannte Dateien ein.</span><span class="sxs-lookup"><span data-stu-id="f60b5-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="f60b5-108">Microsoft Defender for Office 365 scannt nicht jede einzelne Datei in SharePoint Online, OneDrive oder Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f60b5-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="f60b5-109">Dateien werden asynchron durch einen Prozess überprüft, der Freigabe- und Gastaktivitätsereignisse sowie intelligente Heuristiken und Bedrohungssignale verwendet, um schädliche Dateien zu identifizieren.</span><span class="sxs-lookup"><span data-stu-id="f60b5-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="f60b5-110">Weitere [Informationen zu Office 365, SharePoint, OneDrive und](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)Microsoft Teams finden Sie unter Microsoft Defender for Microsoft Teams .</span><span class="sxs-lookup"><span data-stu-id="f60b5-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>