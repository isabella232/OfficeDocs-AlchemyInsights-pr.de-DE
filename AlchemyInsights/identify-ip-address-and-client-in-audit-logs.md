---
title: Identifizieren der IP-Adresse und des Clients in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508915"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="91837-102">Identifizieren der IP-Adresse und des Clients in Überwachungsprotokollen</span><span class="sxs-lookup"><span data-stu-id="91837-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="91837-103">Die IP-Adresse, die einer Aktivität eines Microsoft 365-Benutzers oder-Administrators entspricht, wird in den Überwachungsprotokollen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="91837-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="91837-104">Die Clientinformationen werden ebenfalls protokolliert.</span><span class="sxs-lookup"><span data-stu-id="91837-104">The client information is also logged.</span></span> <span data-ttu-id="91837-105">Hier sind die Schritte zum Identifizieren solcher Informationen.</span><span class="sxs-lookup"><span data-stu-id="91837-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="91837-106">Melden Sie sich beim [Microsoft 365 Security & Compliance Center](https://protection.office.com/)an.</span><span class="sxs-lookup"><span data-stu-id="91837-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="91837-107">Wechseln Sie zur **Search**  >  Suchseite**Überwachungsprotokoll** suchen.</span><span class="sxs-lookup"><span data-stu-id="91837-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="91837-108">Wenn Sie an einer bestimmten Aktivität interessiert sind, wählen Sie diese in der Liste **Aktivitäten** aus.</span><span class="sxs-lookup"><span data-stu-id="91837-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="91837-109">Wenn dies nicht der Fall ist, werden alle Aktivitäten für den ausgewählten Benutzer zurückgegeben (Standardeinstellung).</span><span class="sxs-lookup"><span data-stu-id="91837-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="91837-110">**Hinweis**: bestimmte Aktivitäten stehen im Menü **Aktivitäten** möglicherweise nicht zur Verfügung; Diese Überwachungselemente werden jedoch zurückgegeben, wenn **Ergebnisse für alle Aktivitäten anzeigen** ausgewählt ist (Standardeinstellung).</span><span class="sxs-lookup"><span data-stu-id="91837-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="91837-111">Geben Sie im Feld **Benutzer** den Benutzernamen an, wählen Sie den entsprechenden Datumsbereich für die Aktivität aus, und klicken Sie dann auf **Suchen**.</span><span class="sxs-lookup"><span data-stu-id="91837-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="91837-112">In den Ergebnissen können Sie die IP-Adresse für diese Aktivität im Ergebnisbereich anzeigen.</span><span class="sxs-lookup"><span data-stu-id="91837-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="91837-113">Wählen Sie den Überwachungseintrag aus, um detaillierte Informationen im Flyout **Details** anzuzeigen (beispielsweise Client, Benutzer, der eine Aktion ausgeführt hat, usw.).</span><span class="sxs-lookup"><span data-stu-id="91837-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="91837-114">Weitere Informationen finden Sie unter [Suchen der IP-Adresse des Computers, der für den Zugriff auf ein kompromittiertes Konto verwendet](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)wurde.</span><span class="sxs-lookup"><span data-stu-id="91837-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
