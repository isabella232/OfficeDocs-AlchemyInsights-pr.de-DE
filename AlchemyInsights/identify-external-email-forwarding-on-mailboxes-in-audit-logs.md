---
title: Identifizieren der externen e-Mail-Weiterleitung für Postfächer in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716459"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="4eb93-102">Ermitteln, wann externe e-Mail-Weiterleitung für Postfächer konfiguriert ist</span><span class="sxs-lookup"><span data-stu-id="4eb93-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="4eb93-103">Wenn ein Microsoft 365-Benutzer die externe e-Mail-Weiterleitung für ein Postfach konfiguriert, wird die Aktivität im Rahmen des Cmdlets "Set **-Mailbox** " überwacht.</span><span class="sxs-lookup"><span data-stu-id="4eb93-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="4eb93-104">Sie können die Aktivität mithilfe der Überwachungsprotokoll Suche im Security & Compliance Center anzeigen.</span><span class="sxs-lookup"><span data-stu-id="4eb93-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="4eb93-105">Melden Sie sich beim [Microsoft 365 Security & Compliance Center](https://protection.office.com/)an.</span><span class="sxs-lookup"><span data-stu-id="4eb93-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="4eb93-106">Wechseln Sie zur **Search** > Suchseite**Überwachungsprotokoll** suchen.</span><span class="sxs-lookup"><span data-stu-id="4eb93-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="4eb93-107">Wählen Sie den Datumsbereich in den Feldern **Start Datum** und **Enddatum** aus.</span><span class="sxs-lookup"><span data-stu-id="4eb93-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="4eb93-108">Sie müssen keinen Benutzernamen angeben.</span><span class="sxs-lookup"><span data-stu-id="4eb93-108">You don't need to specify a username.</span></span> <span data-ttu-id="4eb93-109">Stellen Sie sicher, dass das Feld **Aktivitäten** auf **Ergebnisse für alle Aktivitäten anzeigen**festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="4eb93-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="4eb93-110">Klicken Sie auf **Suchen**.</span><span class="sxs-lookup"><span data-stu-id="4eb93-110">Click **Search**.</span></span>

<span data-ttu-id="4eb93-111">Klicken Sie in den Ergebnissen auf **Filterergebnisse** , und geben Sie im Feld Aktivitäts Filter den Text **Satz-Postfach** ein.</span><span class="sxs-lookup"><span data-stu-id="4eb93-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="4eb93-112">Wählen Sie einen Überwachungseintrag in den Ergebnissen aus.</span><span class="sxs-lookup"><span data-stu-id="4eb93-112">Select an audit record in the results.</span></span> <span data-ttu-id="4eb93-113">Klicken Sie im **Detail** Flyout auf **Weitere Informationen**.</span><span class="sxs-lookup"><span data-stu-id="4eb93-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="4eb93-114">Sie müssen sich die Details jedes Überwachungsdatensatzes ansehen, um festzustellen, ob die Aktivität mit der e-Mail-Weiterleitung zusammenhängt.</span><span class="sxs-lookup"><span data-stu-id="4eb93-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="4eb93-115">**ObjectID**: der Alias Wert des Postfachs, das geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="4eb93-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="4eb93-116">**Parameter**: _ForwardingSmtpAddress_ gibt die Ziel-e-Mail-Adresse an.</span><span class="sxs-lookup"><span data-stu-id="4eb93-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="4eb93-117">**UserID**: der Benutzer, der die e-Mail-Weiterleitung für das Postfach im Feld **objectID** konfiguriert hat.</span><span class="sxs-lookup"><span data-stu-id="4eb93-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="4eb93-118">Weitere Informationen finden Sie unter [bestimmen der Personen, die die e-Mail-Weiterleitung für ein Postfach eingerichtet](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)haben.</span><span class="sxs-lookup"><span data-stu-id="4eb93-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
