---
title: Aktivieren von Office 365 ATP für SharePoint, OneDrive und Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403032"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="49ac0-102">Aktivieren von Office 365 Advanced Threat Protection für SharePoint Online, OneDrive und Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="49ac0-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="49ac0-103">Gehen Sie auf https://protection.office.com, und melden Sie sich an.</span><span class="sxs-lookup"><span data-stu-id="49ac0-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="49ac0-104">Wählen Sie**sichere Anlagen**für die **Bedrohungs Verwaltungs** > **Richtlinie** > aus.</span><span class="sxs-lookup"><span data-stu-id="49ac0-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="49ac0-105">Wählen Sie **ATP für SharePoint, OneDrive und Microsoft Teams aktivieren**aus, und klicken Sie dann auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="49ac0-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="49ac0-106">Empfohlen Führen Sie als globaler Administrator oder SharePoint Online-Administrator das Cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) aus, wobei der Parameter **DisallowInfectedFileDownload** auf *true*festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="49ac0-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="49ac0-107">Empfohlen [Richten Sie Warnungen](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) für erkannte Dateien ein.</span><span class="sxs-lookup"><span data-stu-id="49ac0-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="49ac0-108">ATP prüft nicht jede einzelne Datei in SharePoint Online, OneDrive oder Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="49ac0-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="49ac0-109">Dateien werden asynchron durch einen Prozess gescannt, der Freigabe-und Gast Aktivitätsereignisse sowie intelligente Heuristiken und Bedrohungs Signale zur Identifizierung schädlicher Dateien verwendet.</span><span class="sxs-lookup"><span data-stu-id="49ac0-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="49ac0-110">Weitere Informationen finden Sie unter [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="49ac0-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>