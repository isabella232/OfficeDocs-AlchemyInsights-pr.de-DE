---
title: Identifizieren der externen e-Mail-Weiterleitung für Postfächer in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417211"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="41c26-102">Identifizieren, wann externe e-Mail-Weiterleitung für Postfächer konfiguriert ist</span><span class="sxs-lookup"><span data-stu-id="41c26-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="41c26-103">Wenn ein Benutzer die externe e-Mail-Weiterleitung für ein Postfach konfiguriert, wird die Aktivität als Teil des Cmdlets **Set-Mailbox** überwacht.</span><span class="sxs-lookup"><span data-stu-id="41c26-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="41c26-104">Sie können die Aktivität mithilfe der Überwachungsprotokoll Suche im Security & Compliance Center anzeigen.</span><span class="sxs-lookup"><span data-stu-id="41c26-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="41c26-105">Melden Sie sich beim [Office 365 Security _AMP_ Compliance Center](https://protection.office.com/) an.</span><span class="sxs-lookup"><span data-stu-id="41c26-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="41c26-106">Klicken Sie auf **Suchen und Untersuchung** , und wählen Sie **Überwachungsprotokoll Suche**aus.</span><span class="sxs-lookup"><span data-stu-id="41c26-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="41c26-107">Wählen Sie den Datumsbereich in den Feldern **Start Datum** und Enddatum aus. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="41c26-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="41c26-108">Sie müssen keinen Benutzernamen angeben.</span><span class="sxs-lookup"><span data-stu-id="41c26-108">You don't need to specify a username.</span></span> <span data-ttu-id="41c26-109">Stellen Sie sicher, dass das Feld **Aktivitäten** auf **Ergebnisse für alle Aktivitäten anzeigen**festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="41c26-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="41c26-110">Klicken Sie auf **Suchen**.</span><span class="sxs-lookup"><span data-stu-id="41c26-110">Click **Search**.</span></span>

<span data-ttu-id="41c26-111">Klicken Sie in den Ergebnissen auf **Ergebnisse filtern** , und geben Sie **Set-Mailbox** in das Feld Aktivitäts Filter ein.</span><span class="sxs-lookup"><span data-stu-id="41c26-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="41c26-112">Wählen Sie in den Ergebnissen einen Überwachungsdatensatz aus.</span><span class="sxs-lookup"><span data-stu-id="41c26-112">Select an audit record in the results.</span></span> <span data-ttu-id="41c26-113">Klicken Sie im **Detail** Flyout auf **Weitere Informationen**.</span><span class="sxs-lookup"><span data-stu-id="41c26-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="41c26-114">Sie müssen sich die Details der einzelnen Überwachungsdatensätze ansehen, um festzustellen, ob die Aktivität mit der e-Mail-Weiterleitung verbunden ist.</span><span class="sxs-lookup"><span data-stu-id="41c26-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="41c26-115">**ObjectID**: der Alias Wert des Postfachs, das geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="41c26-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="41c26-116">**Parameter**: _ForwardingSmtpAddress_ gibt die Ziel-e-Mail-Adresse an.</span><span class="sxs-lookup"><span data-stu-id="41c26-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="41c26-117">**UserID**: der Benutzer, der die e-Mail-Weiterleitung für das Postfach im **objectID** -Feld konfiguriert hat.</span><span class="sxs-lookup"><span data-stu-id="41c26-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="41c26-118">Weitere Informationen finden Sie unter [bestimmen der Benutzer, die e-Mail-Weiterleitung für ein Postfach eingerichtet](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)haben.</span><span class="sxs-lookup"><span data-stu-id="41c26-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
