---
title: Vorgehensweise hinzufügen oder Entfernen einer Stellvertretung in Outlook für Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571836"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="9e67b-102">Vorgehensweise hinzufügen oder Entfernen einer Stellvertretung in Outlook für Windows</span><span class="sxs-lookup"><span data-stu-id="9e67b-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="9e67b-103">So fügen Sie in Outlook für Windows eine Stellvertretung hinzu:</span><span class="sxs-lookup"><span data-stu-id="9e67b-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="9e67b-104">Klicken Sie auf die Registerkarte **Datei** , gefolgt von den **Kontoeinstellungen**, und wählen Sie dann **Stellvertretungszugriff** aus.</span><span class="sxs-lookup"><span data-stu-id="9e67b-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="9e67b-105">Klicken Sie auf **Hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="9e67b-105">Click on **Add**.</span></span> <span data-ttu-id="9e67b-106">Wenn **Add** nicht angezeigt wird, ist zwischen Outlook und Exchange möglicherweise keine aktive Verbindung vorhanden.</span><span class="sxs-lookup"><span data-stu-id="9e67b-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="9e67b-107">In der Outlook-Statusleiste wird der Verbindungsstatus angezeigt.</span><span class="sxs-lookup"><span data-stu-id="9e67b-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="9e67b-108">Geben Sie den Namen der Person ein, die Sie als Stellvertreter festlegen möchten, oder suchen Sie den Namen in der Liste mit den Suchergebnissen aus, und wählen Sie ihn aus.</span><span class="sxs-lookup"><span data-stu-id="9e67b-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="9e67b-109">Bei der Stellvertretung muss es sich um eine Person in der globalen Exchange-Adressliste (GAL) Ihrer Organisation handeln.</span><span class="sxs-lookup"><span data-stu-id="9e67b-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="9e67b-110">Klicken Sie auf **Hinzufügen** , gefolgt von **OK**.</span><span class="sxs-lookup"><span data-stu-id="9e67b-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="9e67b-111">Übernehmen Sie im Dialogfeld **Berechtigungen delegieren** die Standard Berechtigungseinstellungen, oder wählen Sie benutzerdefinierte Zugriffsebenen für Exchange-Ordner aus.</span><span class="sxs-lookup"><span data-stu-id="9e67b-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="9e67b-112">Wenn ein Stellvertreter die Berechtigung zum Arbeiten nur mit Besprechungsanfragen und-Antworten benötigt, werden die Standard Berechtigungseinstellungen wie **Stellvertreter Kopien von Besprechungs bezogenen Nachrichten erhalten, die an mich gesendet** wurden, genügen.</span><span class="sxs-lookup"><span data-stu-id="9e67b-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="9e67b-113">Sie können die Einstellung **Posteingangs** Berechtigung auf **None** belassen.</span><span class="sxs-lookup"><span data-stu-id="9e67b-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="9e67b-114">Besprechungsanfragen und-Antworten gelangen direkt in den Posteingang des Stellvertreters.</span><span class="sxs-lookup"><span data-stu-id="9e67b-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="9e67b-115">Standardmäßig wird der Stellvertretung die Berechtigung **Editor (Elemente lesen, erstellen und ändern)** für den Ordner **Kalender** erteilt.</span><span class="sxs-lookup"><span data-stu-id="9e67b-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="9e67b-116">Wenn der Stellvertreter auf eine Besprechung in Ihrem Namen antwortet, wird dieser automatisch Ihrem **Kalender** Ordner hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="9e67b-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="9e67b-117">Um eine Nachricht zu senden, um die Stellvertretung über die geänderten Berechtigungen zu benachrichtigen, aktivieren Sie das Kontrollkästchen **eine Nachricht wird automatisch an delegierende dieser Berechtigungen gesendet** .</span><span class="sxs-lookup"><span data-stu-id="9e67b-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="9e67b-118">Wenn Sie möchten, aktivieren Sie das Kontrollkästchen **Stellvertretung kann private Elemente anzeigen** .</span><span class="sxs-lookup"><span data-stu-id="9e67b-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="9e67b-119">Diese Einstellung wirkt sich auf alle Exchange-Ordner aus.</span><span class="sxs-lookup"><span data-stu-id="9e67b-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="9e67b-120">Dies umfasst alle Ordner "e-Mail", "Kontakte", "Kalender", "Aufgaben", "Notizen" und "Journal".</span><span class="sxs-lookup"><span data-stu-id="9e67b-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="9e67b-121">Es gibt keine Möglichkeit, privaten Elementen nur in bestimmten Ordnern Zugriff zu gewähren.</span><span class="sxs-lookup"><span data-stu-id="9e67b-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="9e67b-122">Wählen Sie **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="9e67b-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="9e67b-123">Nachrichten, die mit Berechtigungen zum Senden im Auftrag von gesendet werden, umfassen sowohl die Stellvertretung als auch ihre Namen neben **aus**.</span><span class="sxs-lookup"><span data-stu-id="9e67b-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="9e67b-124">Wenn eine Nachricht mit "Senden als"-Berechtigungen gesendet wird, wird nur Ihr Name angezeigt.</span><span class="sxs-lookup"><span data-stu-id="9e67b-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="9e67b-125">Nachdem Sie eine Person als Stellvertretung hinzugefügt haben, können Sie Ihr Exchange-Postfach Ihrem Outlook-Profil hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="9e67b-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="9e67b-126">Anweisungen finden Sie unter [Verwalten der e-Mails und Kalenderelemente einer anderen Person](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span><span class="sxs-lookup"><span data-stu-id="9e67b-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="9e67b-127">So entfernen Sie eine Stellvertretung in Outlook für Windows:</span><span class="sxs-lookup"><span data-stu-id="9e67b-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="9e67b-128">Klicken Sie auf die Registerkarte **Datei** .</span><span class="sxs-lookup"><span data-stu-id="9e67b-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="9e67b-129">Klicken Sie auf **Kontoeinstellungen** gefolgt von **Stellvertretungszugriff**.</span><span class="sxs-lookup"><span data-stu-id="9e67b-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="9e67b-130">Wählen Sie den Namen des Stellvertreters aus, für den Sie Berechtigungen ändern möchten, und klicken Sie dann auf **Entfernen** , gefolgt von **OK**.</span><span class="sxs-lookup"><span data-stu-id="9e67b-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
