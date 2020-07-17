---
title: Erstellen einer Freigaberichtlinie, um Ihren Benutzern die Freigabe ihrer Kalenderdaten für Personen außerhalb Ihrer Organisation zu erlauben
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cb2c0af55f4f8833709b6952d3a6e2ac258ce5fc
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/23/2020
ms.locfileid: "44854018"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a><span data-ttu-id="952d6-102">Erstellen einer Freigaberichtlinie, um Ihren Benutzern die Freigabe ihrer Kalenderdaten für Personen außerhalb Ihrer Organisation zu erlauben</span><span class="sxs-lookup"><span data-stu-id="952d6-102">Create a Sharing Policy to allow your users to share their calendar with people outside your organization</span></span>

1. <span data-ttu-id="952d6-103">Wechseln Sie vom Microsoft 365 Admin Center-Dashboards zu **Admin** > **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="952d6-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="952d6-104">Wechseln Sie zu **Organisation** > **Freigabe**.</span><span class="sxs-lookup"><span data-stu-id="952d6-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="952d6-105">Klicken Sie in der Listenansicht unter **Einzelne Freigabe** auf **Neu**.</span><span class="sxs-lookup"><span data-stu-id="952d6-105">In the list view, under **Individual Sharing**, click **New** .</span></span>
4. <span data-ttu-id="952d6-106">Geben Sie unter **Neue Freigaberichtlinie** einen Anzeigenamen für die Freigaberichtlinie im Feld **Richtlinienname** ein.</span><span class="sxs-lookup"><span data-stu-id="952d6-106">In **new sharing policy**, type a friendly name for the sharing policy in the **Policy name** box.</span></span>
5. <span data-ttu-id="952d6-107">Klicken Sie auf **Hinzufügen**, um die Freigaberegeln für die Richtlinie zu definieren.</span><span class="sxs-lookup"><span data-stu-id="952d6-107">Click **Add**  to define the sharing rules for the policy.</span></span>
6. <span data-ttu-id="952d6-108">Wählen Sie im Dialogfeld **Freigaberegel** eine der folgenden Optionen aus, um die Domänen für die Freigabe anzugeben:</span><span class="sxs-lookup"><span data-stu-id="952d6-108">In **sharing rule**, select one of the following options to specify the domains you want to share with:</span></span>
    - <span data-ttu-id="952d6-109">**Freigabe für alle Domänen**</span><span class="sxs-lookup"><span data-stu-id="952d6-109">**Sharing with all domains**</span></span>
    - <span data-ttu-id="952d6-110">**Freigabe für eine bestimmte Domäne**</span><span class="sxs-lookup"><span data-stu-id="952d6-110">**Sharing with a specific domain**</span></span>
8. <span data-ttu-id="952d6-p101">Wenn Sie **Freigabe für eine bestimmte Domäne** auswählen, geben Sie die Domäne für die Freigabe ein. Wenn Sie mehr als eine Domäne für diese Freigaberichtlinie eingeben müssen, speichern Sie zunächst die Einstellungen für die erste Domäne. Bearbeiten Sie anschließend die Freigaberegeln, um weitere Domänen hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="952d6-p101">If you select **Sharing with a specific domain**, type the name of the domain you want to share with. If you need to enter more than one domain for this sharing policy, save the settings for the first domain, then edit the sharing rules to add more domains.</span></span>
9. <span data-ttu-id="952d6-113">Zum Angeben der freizugebenden Informationen aktivieren Sie das Kontrollkästchen **Ihre Kalenderordner freigeben**. Wählen Sie anschließend eine der folgenden Optionen aus:</span><span class="sxs-lookup"><span data-stu-id="952d6-113">To specify the information that can be shared, select the **Share your calendar folder** check box, and then select one of the following options:</span></span>
    - <span data-ttu-id="952d6-114">**Frei/Gebucht-Kalenderinformationen nur mit Zeit**</span><span class="sxs-lookup"><span data-stu-id="952d6-114">**Calendar free/busy information with time only**</span></span>
    - <span data-ttu-id="952d6-115">**Frei/Gebucht-Kalenderinformationen mit Zeit, Betreff und Ort**</span><span class="sxs-lookup"><span data-stu-id="952d6-115">**Calendar free/busy information with time, subject, and location**</span></span>
    - <span data-ttu-id="952d6-116">**Alle Informationen zum Termin einschließlich Uhrzeit, Betreff, Ort und Titel**</span><span class="sxs-lookup"><span data-stu-id="952d6-116">**All calendar appointment information, including time, subject, location and title**</span></span>
11. <span data-ttu-id="952d6-117">Klicken Sie auf **Speichern**, um die Regeln für die Freigaberichtlinie festzulegen.</span><span class="sxs-lookup"><span data-stu-id="952d6-117">Click **save** to set the rules for the sharing policy.</span></span>
12. <span data-ttu-id="952d6-118">Wenn Sie diese Freigaberichtlinie als die neue Standardfreigaberichtlinie für alle Benutzer in Ihrer Organisation festlegen möchten, aktivieren Sie das Kontrollkästchen **Diese Richtlinie als meine Standardfreigaberichtlinie verwenden**.</span><span class="sxs-lookup"><span data-stu-id="952d6-118">If you want to set this sharing policy as the new default sharing policy for all users in your organization, select the **Make this policy my default sharing policy** check box.</span></span>
13. <span data-ttu-id="952d6-119">Klicken Sie auf **Speichern**, um die Freigaberichtlinie zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="952d6-119">Click **save** to create the sharing policy.</span></span>  

<span data-ttu-id="952d6-120">**Für vollständige Informationen zu diesem Thema lesen Sie:**</span><span class="sxs-lookup"><span data-stu-id="952d6-120">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="952d6-121">Erstellen einer Freigaberichtlinie in Exchange Online</span><span class="sxs-lookup"><span data-stu-id="952d6-121">Create a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [<span data-ttu-id="952d6-122">Anwenden von Freigaberichtlinien auf Postfächer in Exchange Online</span><span class="sxs-lookup"><span data-stu-id="952d6-122">Apply a sharing policy to mailboxes in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [<span data-ttu-id="952d6-123">Ändern, Deaktivieren oder Entfernen einer Freigaberichtlinie in Exchange Online</span><span class="sxs-lookup"><span data-stu-id="952d6-123">Modify, disable, or remove a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)