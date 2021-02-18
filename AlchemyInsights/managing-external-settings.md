---
title: Externe Einstellungen verwalten
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/17/2021
ms.locfileid: "50282836"
---
# <a name="managing-external-settings"></a><span data-ttu-id="bc5fd-102">Externe Einstellungen verwalten</span><span class="sxs-lookup"><span data-stu-id="bc5fd-102">Managing External Settings</span></span>

<span data-ttu-id="bc5fd-103">**Ankündigung**</span><span class="sxs-lookup"><span data-stu-id="bc5fd-103">**Announcement**</span></span>

- <span data-ttu-id="bc5fd-104">[Die Einstellung der WebView-Anmeldeunterstützung von Google beginnt ab dem 4. Januar 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span><span class="sxs-lookup"><span data-stu-id="bc5fd-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="bc5fd-105">Testen Sie, ob Ihre Apps betroffen sind, indem Sie die Anweisungen von Google zum Testen der Kompatibilität befolgen</span><span class="sxs-lookup"><span data-stu-id="bc5fd-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="bc5fd-106">Stellen Sie sicher, dass Sie die Systemwebansicht oder den Systembrowser verwenden, wenn Sie Ihre Benutzer mit Google-Heimanwenderkonten anmelden.</span><span class="sxs-lookup"><span data-stu-id="bc5fd-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="bc5fd-107">**Einladungseinstellungen verwalten**</span><span class="sxs-lookup"><span data-stu-id="bc5fd-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="bc5fd-108">Stellen Sie sicher, dass Sie die [Einstellungen für die externe Zusammenarbeit konfiguriert haben](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support), damit die entsprechenden Personen Einladungen senden können.</span><span class="sxs-lookup"><span data-stu-id="bc5fd-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="bc5fd-109">**Zugriffsberechtigungen für Gastbenutzer verwalten**</span><span class="sxs-lookup"><span data-stu-id="bc5fd-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="bc5fd-110">Globale Administratoren können Zugriffsberechtigungen für Gäste im Verzeichnis über das Azure-Portal verwalten, indem sie die Gastzugriffsberechtigungen auf der Seite „Einstellungen für die externe Zusammenarbeit“ konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="bc5fd-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="bc5fd-111">[Erfahren Sie mehr über diese Einstellung](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="bc5fd-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="bc5fd-112">Wenn Sie möchten, dass Ihre Gäste auf Apps wie Teams oder SharePoint zugreifen können, bestätigen Sie, dass Sie diese Apps so konfiguriert haben, dass der Gastzugriff ermöglicht ist.</span><span class="sxs-lookup"><span data-stu-id="bc5fd-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="bc5fd-113">Erfahren Sie mehr über die [Teams-Einstellungen](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) und [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="bc5fd-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="bc5fd-114">**Einladungen konfigurieren:**</span><span class="sxs-lookup"><span data-stu-id="bc5fd-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="bc5fd-115">Aktivieren der externen B2B-Zusammenarbeit und Verwalten, wer Gäste einladen kann</span><span class="sxs-lookup"><span data-stu-id="bc5fd-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="bc5fd-116">Zulassen oder Blockieren von Einladungen für Benutzer von bestimmten Organisationen</span><span class="sxs-lookup"><span data-stu-id="bc5fd-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="bc5fd-117">**Konfigurieren der zugelassenen Identitätsanbieter:**</span><span class="sxs-lookup"><span data-stu-id="bc5fd-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="bc5fd-118">Google Partnerverbund</span><span class="sxs-lookup"><span data-stu-id="bc5fd-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="bc5fd-119">Direkter Partnerverbund</span><span class="sxs-lookup"><span data-stu-id="bc5fd-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="bc5fd-120">Authentifizierung mit Einmalkennung über E-Mail</span><span class="sxs-lookup"><span data-stu-id="bc5fd-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
