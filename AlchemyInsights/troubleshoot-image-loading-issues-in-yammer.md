---
title: Behandeln von Problemen beim Laden von Bildern in Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: cf330adbf3f3a92d4b90768c7dd8bada6333db80
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690242"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="90dd0-102">Behandeln von Problemen beim Laden von Bildern in Yammer</span><span class="sxs-lookup"><span data-stu-id="90dd0-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="90dd0-103">Wenn in Yammer Probleme mit Fotos und der Dateivorschau auftreten, können Sie diese beheben, indem Sie überprüfen, ob das Problem für alle Benutzer auftritt, ob es auf mobilen Geräten geschieht, und ob es beim Hochladen der Anlage reproduzierbar ist.</span><span class="sxs-lookup"><span data-stu-id="90dd0-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="90dd0-104">**Probleme mit dem Profilfoto**</span><span class="sxs-lookup"><span data-stu-id="90dd0-104">**Profile photo issues**</span></span>  

<span data-ttu-id="90dd0-105">Wenn sich Endbenutzer über Microsoft 365 bei Yammer anmelden, müssen sie ihr Profil einschließlich des Profilfotos ändern.</span><span class="sxs-lookup"><span data-stu-id="90dd0-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="90dd0-106">Wenn Benutzer keine Profilupdates vornehmen dürfen, kann ein Administrator das Update für den Benutzer vornehmen.</span><span class="sxs-lookup"><span data-stu-id="90dd0-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="90dd0-107">Weitere Informationen finden Sie unter [Anzeigen und Aktualisieren Ihres Profils in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="90dd0-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="90dd0-108">Informationen zum Bearbeiten des Profils, einschließlich der Profilfotos, finden Sie unter [Ändern des Yammer-Profils und der Yammer-Einstellungen](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="90dd0-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="90dd0-109">Aktualisierte Profilfotos werden anders synchronisiert als Profilattribute.</span><span class="sxs-lookup"><span data-stu-id="90dd0-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="90dd0-110">Benutzer müssen sich anmelden, um eine Synchronisierung Ihres Profilfotos zu initiieren.</span><span class="sxs-lookup"><span data-stu-id="90dd0-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="90dd0-111">Informationen finden Sie unter [Werden Benutzerprofilbilder aus Office 365 in Yammer aktualisiert?](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="90dd0-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="90dd0-112">Informationen zum Benutzerlebenszyklus für Yammer finden Sie unter [Verwalten von Yammer-Benutzern über ihren gesamten Lebenszyklus in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="90dd0-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="90dd0-113">Einzelheiten dazu, wie die Profilbildsynchronisierung in Microsoft 365 funktioniert, finden Sie unter [Informationen zur Profilbildsynchronisierung in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="90dd0-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="90dd0-114">**Probleme mit der Dokumentvorschau und der Miniaturansicht von Bildern**</span><span class="sxs-lookup"><span data-stu-id="90dd0-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="90dd0-115">Wenn Dateien oder Bilder in Yammer gepostet werden, werden Vorschauoptionen möglicherweise aus den folgenden Gründen nicht angezeigt:</span><span class="sxs-lookup"><span data-stu-id="90dd0-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="90dd0-116">Die Datei ist beschädigt und kann nicht geöffnet verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="90dd0-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="90dd0-117">Die Datei wurde nicht kürzlich in SharePoint Online hochgeladen, oder Yammer verfügt aus anderen Gründen über ungültige Metadaten.</span><span class="sxs-lookup"><span data-stu-id="90dd0-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="90dd0-118">URLs, die zum Laden der Vorschaubilder erforderlich sind, werden blockiert.</span><span class="sxs-lookup"><span data-stu-id="90dd0-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="90dd0-119">Die Dateivorschau wurde vom Benutzer vor dem Posten entfernt.</span><span class="sxs-lookup"><span data-stu-id="90dd0-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="90dd0-120">Ein Problem mit dem Dienst hat die Generierung einer Vorschau verhindert.</span><span class="sxs-lookup"><span data-stu-id="90dd0-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="90dd0-121">**Hinweis** Vorschauen für Links und Dateiuploads können sich anders verhalten.</span><span class="sxs-lookup"><span data-stu-id="90dd0-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="90dd0-122">Links zu Dateien im Internet oder Links, für die eine zusätzliche Authentifizierung erforderlich ist, werden möglicherweise nicht ordnungsgemäß angezeigt.</span><span class="sxs-lookup"><span data-stu-id="90dd0-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="90dd0-123">Weitere Informationen hierzu finden Sie unter [Anfügen einer Datei oder eines Bilds an eine Yammer-Nachricht](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="90dd0-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 