---
title: Identifizieren der IP-Adresse und des Clients in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: a91778c006531371b85116f5c97485d42e6cc5be
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35382952"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="c2062-102">Identifizieren der IP-Adresse und des Clients in Überwachungsprotokollen</span><span class="sxs-lookup"><span data-stu-id="c2062-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="c2062-103">Die IP-Adresse, die einer Aktivität durch einen Benutzer oder Administrator entspricht, wird in den Überwachungsprotokollen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="c2062-103">The IP address that corresponds to an activity by a user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="c2062-104">Die Clientinformationen werden ebenfalls protokolliert.</span><span class="sxs-lookup"><span data-stu-id="c2062-104">The client information is also logged.</span></span> <span data-ttu-id="c2062-105">Hier sind die Schritte zum Identifizieren solcher Informationen.</span><span class="sxs-lookup"><span data-stu-id="c2062-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="c2062-106">Melden Sie sich beim [Office 365 Security #a0 Compliance Center](https://protection.office.com/) an.</span><span class="sxs-lookup"><span data-stu-id="c2062-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="c2062-107">Klicken Sie auf **Suche und Untersuchung** , und wählen Sie **Überwachungsprotokoll Suche**aus.</span><span class="sxs-lookup"><span data-stu-id="c2062-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

   <span data-ttu-id="c2062-108">Wenn Sie an einer bestimmten Aktivität interessiert sind, wählen Sie diese in der Liste **Aktivitäten** aus.</span><span class="sxs-lookup"><span data-stu-id="c2062-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="c2062-109">Wenn dies nicht der Fall ist, werden alle Aktivitäten für den ausgewählten Benutzer zurückgegeben (Standardeinstellung).</span><span class="sxs-lookup"><span data-stu-id="c2062-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="c2062-110">**Hinweis**: bestimmte Aktivitäten stehen im Menü **Aktivitäten** möglicherweise nicht zur Verfügung; Diese Überwachungselemente werden jedoch zurückgegeben, wenn **Ergebnisse für alle Aktivitäten anzeigen** ausgewählt ist (Standardeinstellung).</span><span class="sxs-lookup"><span data-stu-id="c2062-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="c2062-111">Geben Sie im Feld **Benutzer** den Benutzernamen an, wählen Sie den entsprechenden Datumsbereich für die Aktivität aus, und klicken Sie dann auf **Suchen**.</span><span class="sxs-lookup"><span data-stu-id="c2062-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="c2062-112">In den Ergebnissen können Sie die IP-Adresse für diese Aktivität im Ergebnisbereich anzeigen.</span><span class="sxs-lookup"><span data-stu-id="c2062-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="c2062-113">Wählen Sie den Überwachungseintrag aus, um detaillierte Informationen im Flyout **Details** anzuzeigen (beispielsweise Client, Benutzer, der eine Aktion ausgeführt hat, usw.).</span><span class="sxs-lookup"><span data-stu-id="c2062-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="c2062-114">Weitere Informationen finden Sie unter [Suchen der IP-Adresse des Computers, der für den Zugriff auf ein kompromittiertes Konto verwendet](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)wurde.</span><span class="sxs-lookup"><span data-stu-id="c2062-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
