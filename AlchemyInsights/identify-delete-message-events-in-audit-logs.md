---
title: Identifizieren von Ereignissen zum Löschen von Nachrichten in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 0fb5d6aa0c99f7f68459c40302869bed69583b3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755152"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="9ea4f-102">Überwachungsprotokolle für gelöschte e-Mail-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="9ea4f-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="9ea4f-103">Ab Januar 2019 wendet Microsoft die postfachüberwachungsprotokollierung standardmäßig an.</span><span class="sxs-lookup"><span data-stu-id="9ea4f-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="9ea4f-104">Andernfalls müssen Sie die Löschaktionen für die Überwachung manuell aktivieren, um Lösch Nachrichten Ereignisse für einen bestimmten Benutzer zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="9ea4f-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="9ea4f-105">Wenn die postfachüberwachungsprotokollierung bereits für Ihre Organisation oder für den jeweiligen Benutzer aktiviert ist, führen Sie die folgenden Schritte aus.</span><span class="sxs-lookup"><span data-stu-id="9ea4f-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="9ea4f-106">Melden Sie sich beim [Office 365 Security #a0 Compliance Center](https://protection.office.com/) an.</span><span class="sxs-lookup"><span data-stu-id="9ea4f-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="9ea4f-107">Klicken Sie auf **Suche und Untersuchung** , und wählen Sie **Überwachungsprotokoll Suche**aus.</span><span class="sxs-lookup"><span data-stu-id="9ea4f-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="9ea4f-108">Wählen Sie den Datumsbereich in den Feldern **Start Datum** und Enddatum aus. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="9ea4f-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="9ea4f-109">Geben Sie den Benutzernamen für den Benutzer an, der untersucht werden soll (der Benutzer, der die Elemente gelöscht hat).</span><span class="sxs-lookup"><span data-stu-id="9ea4f-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="9ea4f-110">Wählen Sie im Feld **Aktivitäten** die Option **Gelöschte Nachrichten aus dem Ordner "Gelöschte Elemente" aus** , und **Verschieben von Nachrichten in den Ordner "Gelöschte Elemente"**.</span><span class="sxs-lookup"><span data-stu-id="9ea4f-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="9ea4f-111">Klicken Sie auf **Suchen**.</span><span class="sxs-lookup"><span data-stu-id="9ea4f-111">Click **Search**.</span></span>

<span data-ttu-id="9ea4f-112">Wählen Sie in den Ergebnissen einen Überwachungseintrag aus.</span><span class="sxs-lookup"><span data-stu-id="9ea4f-112">In the results, select an audit record.</span></span> <span data-ttu-id="9ea4f-113">Klicken Sie im Detail Flyout auf **Weitere Informationen**.</span><span class="sxs-lookup"><span data-stu-id="9ea4f-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="9ea4f-114">Weitere Informationen zum gelöschten Element (beispielsweise die Betreffzeile und der Speicherort des Elements, wenn es gelöscht wurde) werden im Feld **AffectedItems** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="9ea4f-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="9ea4f-115">Die **ClientInfoString** -Eigenschaft zeigt an, ob der Löschvorgang in Outlook, Outlook im Internet (früher bekannt als Outlook Web App) oder auf einem anderen Gerät aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="9ea4f-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="9ea4f-116">Weitere Informationen finden Sie unter [bestimmen der Personen, die die e-Mail-Weiterleitung für ein Postfach eingerichtet](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items)haben.</span><span class="sxs-lookup"><span data-stu-id="9ea4f-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="9ea4f-117">**Hinweis**: Gelöschte Elemente können nicht mithilfe der Überwachungsprotokoll Funktion abgerufen werden.</span><span class="sxs-lookup"><span data-stu-id="9ea4f-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="9ea4f-118">Informationen zum Abrufen von gelöschten Nachrichten in Outlook im Internet finden Sie unter [Wiederherstellen gelöschter Elemente in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="9ea4f-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
