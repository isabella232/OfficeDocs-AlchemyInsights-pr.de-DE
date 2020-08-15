---
title: Ändern von Updatekanälen für Office-Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 3e1042a38d2289b9ef2396e8300d32f20ddaa703
ms.sourcegitcommit: b5e5f560bf6ef92b4475bd3d91b7df38b5a4b036
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/14/2020
ms.locfileid: "46739826"
---
# <a name="change-update-channels-for-office-apps"></a><span data-ttu-id="21f77-102">Ändern von Updatekanälen für Office-Apps</span><span class="sxs-lookup"><span data-stu-id="21f77-102">Change update channels for Office apps</span></span>

<span data-ttu-id="21f77-103">Bei neuen Office-Installationen verwenden Sie die Office-Software-Downloadeinstellungen, um den gewünschten Updatekanal auszuwählen, und installieren Sie dann Office-Apps (oder installieren Sie sie erneut).</span><span class="sxs-lookup"><span data-stu-id="21f77-103">For new Office installations, use Office Software Download Settings to select the desired update channel, and then install (or re-install) Office apps.</span></span> <span data-ttu-id="21f77-104">Weitere Informationen finden Sie unter [Verwalten von Software-Downloadeinstellungen in Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365).</span><span class="sxs-lookup"><span data-stu-id="21f77-104">For more info, see [Manage software download settings in Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365).</span></span> 

<span data-ttu-id="21f77-105">**Hinweis**: Der über die Office-Software-Downloadeinstellungen ausgewählte Updatekanal gilt für alle Benutzer, die Neuinstallationen über das O365-Portal ausführen.</span><span class="sxs-lookup"><span data-stu-id="21f77-105">**Note** The update channel selected using the Office Software Download Settings applies to all users performing new installations using the O365 portal.</span></span> <span data-ttu-id="21f77-106">Weitere Informationen finden Sie unter [Herunterladen und Installieren oder erneutes Installieren von Microsoft 365 oder Office 2019 auf einem PC oder Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).</span><span class="sxs-lookup"><span data-stu-id="21f77-106">For more info, see [Download and install or reinstall Microsoft 365 or Office 2019 on a PC or Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).</span></span>   

<span data-ttu-id="21f77-107">Für vorhandene Office-Installationen verwenden Sie das Office-Bereitstellungstool (ODT), um zu einem anderen Updatekanal zu wechseln:</span><span class="sxs-lookup"><span data-stu-id="21f77-107">For existing Office installations, use the Office Deployment Tool (ODT) to switch to a different update channel:</span></span>  

1. <span data-ttu-id="21f77-108">Laden Sie die neueste Version des Office-Bereitstellungstools (setup.exe) aus dem [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065) herunter.</span><span class="sxs-lookup"><span data-stu-id="21f77-108">Download the latest version of the Office Deployment Tool (setup.exe) from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
2. <span data-ttu-id="21f77-109">Identifizieren Sie den Namen des Kanals, zu dem Sie wechseln möchten.</span><span class="sxs-lookup"><span data-stu-id="21f77-109">Identify the name of the channel that you want to switch to.</span></span> <span data-ttu-id="21f77-110">Weitere Informationen finden Sie unter [Konfigurationsoptionen für das Office-Bereitstellungstool](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).</span><span class="sxs-lookup"><span data-stu-id="21f77-110">For more info, see [Configuration options for the Office Deployment Tool](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).</span></span>
3. <span data-ttu-id="21f77-111">Erstellen Sie eine XML-Konfigurationsdatei, und geben Sie den entsprechenden Kanalnamen an, z. B. „update.xml“.</span><span class="sxs-lookup"><span data-stu-id="21f77-111">Create a configuration XML file specifying the appropriate channel name, for example, update.xml.</span></span>  

`<Configuration>`<br>
`<Updates Channel="Monthly"/>`<br>
`</Configuration>`<br>

4. <span data-ttu-id="21f77-112">Wechseln Sie von einer Eingabeaufforderung mit erhöhten Rechten zu dem Ordnerspeicherort, an dem sich „setup.exe“ befindet, und führen Sie den folgenden Befehl aus:</span><span class="sxs-lookup"><span data-stu-id="21f77-112">From an elevated command prompt, switch to the folder location where setup.exe resides and run the following command:</span></span>  
    <span data-ttu-id="21f77-113">a.</span><span class="sxs-lookup"><span data-stu-id="21f77-113">a.</span></span> <span data-ttu-id="21f77-114">setup.exe /configure update.xml</span><span class="sxs-lookup"><span data-stu-id="21f77-114">setup.exe /configure update.xml</span></span>
5. <span data-ttu-id="21f77-115">Starten Sie eine Office-Anwendung (z. B. Excel), und wählen Sie dann **Datei** > **Konto** aus.</span><span class="sxs-lookup"><span data-stu-id="21f77-115">Start an Office application (such as Excel), and then select **File** > **Account**.</span></span> <span data-ttu-id="21f77-116">Wählen Sie im Abschnitt „Produktinformationen“ **Updateoptionen** > **Jetzt aktualisieren** aus.</span><span class="sxs-lookup"><span data-stu-id="21f77-116">In the Product Information section, select **Update Options** > **Update Now**.</span></span>

<span data-ttu-id="21f77-117">Weitere Informationen finden Sie unter [Wechseln von Updatekanälen für vorhandene Office-Apps](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel).</span><span class="sxs-lookup"><span data-stu-id="21f77-117">For more information, see [How to switch update channels for existing Office Apps](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel).</span></span> 

<span data-ttu-id="21f77-118">Um Updatekanäle für eine ausgewählte Gruppe von Benutzern oder mithilfe von Configuration Manager (SCCM) zu wechseln, konfigurieren Sie die Einstellung für den Updatekanal mithilfe des Gruppenrichtlinienobjekts (GPO).</span><span class="sxs-lookup"><span data-stu-id="21f77-118">For switching update channels for a selected group of users or by using Configuration Manager (SCCM), configure the Update Channel setting using GPO.</span></span> <span data-ttu-id="21f77-119">Weitere Informationen finden Sie unter [Übersicht über die Updatekanäle für Microsoft 365-Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy).</span><span class="sxs-lookup"><span data-stu-id="21f77-119">For more info, see [Overview of update channels for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy).</span></span> <span data-ttu-id="21f77-120">Weitere Details finden Sie unter [Verwalten von Office 365 ProPlus-Kanälen für IT-Experten](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) und [Verwalten von Updates für Microsoft 365-Apps mithilfe des Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="21f77-120">For details, see [How to manage Office 365 ProPlus Channels for IT Pros](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) and [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).</span></span>