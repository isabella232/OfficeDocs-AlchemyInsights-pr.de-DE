---
title: Steuern automatischer Updates für Office-Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: ab3d6e60bc1b67220adbdf7ba61599a6b7aa663a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747775"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="2316b-102">Steuern automatischer Updates für Office-Apps</span><span class="sxs-lookup"><span data-stu-id="2316b-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="2316b-103">Standardmäßig werden Updates für Office-Apps automatisch heruntergeladen und im Hintergrund angewendet, und zwar ohne Eingriff von Benutzern.</span><span class="sxs-lookup"><span data-stu-id="2316b-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="2316b-104">Administratoren können jedoch mithilfe der Office-Updateeinstellungen steuern, wie Updates angewendet werden.</span><span class="sxs-lookup"><span data-stu-id="2316b-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="2316b-105">Mithilfe der Updateeinstellungen können Administratoren automatische Updates aktivieren oder deaktivieren, die Schaltfläche **Jetzt aktualisieren** in Office ein- oder ausblenden, Updatestichtage festlegen und vieles mehr.</span><span class="sxs-lookup"><span data-stu-id="2316b-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="2316b-106">Ausführliche Informationen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="2316b-106">For detailed information, see:</span></span>

- [<span data-ttu-id="2316b-107">Konfigurieren von Updateeinstellungen für Office</span><span class="sxs-lookup"><span data-stu-id="2316b-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="2316b-108">Automatische Aktualisierung für Office ist nicht aktiviert</span><span class="sxs-lookup"><span data-stu-id="2316b-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="2316b-109">Definieren, wie Office nach der Installation aktualisiert wird</span><span class="sxs-lookup"><span data-stu-id="2316b-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="2316b-110">Um die bestehenden Updateeinstellungen zu überprüfen, die auf einen Clientcomputer angewendet werden, führen Sie diese Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="2316b-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="2316b-111">Öffnen Sie den Registrierungs-Editor über **Start** > **Ausführen** > **regedit**.</span><span class="sxs-lookup"><span data-stu-id="2316b-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="2316b-112">Wechseln Sie zu folgendem Speicherort, und überprüfen Sie die Einstellungen von Office Update:</span><span class="sxs-lookup"><span data-stu-id="2316b-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="2316b-113">a.</span><span class="sxs-lookup"><span data-stu-id="2316b-113">a.</span></span> <span data-ttu-id="2316b-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="2316b-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="2316b-115">b.</span><span class="sxs-lookup"><span data-stu-id="2316b-115">b.</span></span> <span data-ttu-id="2316b-116">ClickToRun\Configuration</span><span class="sxs-lookup"><span data-stu-id="2316b-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="2316b-117">**Hinweis** Wenn der OfficeMgmtCOM-Schlüssel festgelegt ist, wird unter **Office** > **Konto** > **Office-Updates** möglicherweise die Meldung "Updates werden von Ihrem Systemadministrator verwaltet" angezeigt.</span><span class="sxs-lookup"><span data-stu-id="2316b-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="2316b-118">Weitere Informationen finden Sie unter [Verwalten von Updates für Microsoft 365 Apps mithilfe des Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="2316b-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  