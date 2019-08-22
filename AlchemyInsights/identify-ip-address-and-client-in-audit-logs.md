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
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539028"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="27c18-102">Identifizieren der IP-Adresse und des Clients in Überwachungsprotokollen</span><span class="sxs-lookup"><span data-stu-id="27c18-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="27c18-103">Die IP-Adresse, die einer Aktivität eines Office 365 Benutzers oder Administrators entspricht, wird in den Überwachungsprotokollen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="27c18-103">The IP address that corresponds to an activity by an Office 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="27c18-104">Die Clientinformationen werden ebenfalls protokolliert.</span><span class="sxs-lookup"><span data-stu-id="27c18-104">The client information is also logged.</span></span> <span data-ttu-id="27c18-105">Hier sind die Schritte zum Identifizieren solcher Informationen.</span><span class="sxs-lookup"><span data-stu-id="27c18-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="27c18-106">Melden Sie sich beim [Office 365 Security #a0 Compliance Center](https://protection.office.com/)an.</span><span class="sxs-lookup"><span data-stu-id="27c18-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="27c18-107">Wechseln Sie zur \*\*\*\* > Suchseite**Überwachungsprotokoll** suchen.</span><span class="sxs-lookup"><span data-stu-id="27c18-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="27c18-108">Wenn Sie an einer bestimmten Aktivität interessiert sind, wählen Sie diese in der Liste **Aktivitäten** aus.</span><span class="sxs-lookup"><span data-stu-id="27c18-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="27c18-109">Wenn dies nicht der Fall ist, werden alle Aktivitäten für den ausgewählten Benutzer zurückgegeben (Standardeinstellung).</span><span class="sxs-lookup"><span data-stu-id="27c18-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="27c18-110">**Hinweis**: bestimmte Aktivitäten stehen im Menü **Aktivitäten** möglicherweise nicht zur Verfügung; Diese Überwachungselemente werden jedoch zurückgegeben, wenn **Ergebnisse für alle Aktivitäten anzeigen** ausgewählt ist (Standardeinstellung).</span><span class="sxs-lookup"><span data-stu-id="27c18-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="27c18-111">Geben Sie im Feld **Benutzer** den Benutzernamen an, wählen Sie den entsprechenden Datumsbereich für die Aktivität aus, und klicken Sie dann auf **Suchen**.</span><span class="sxs-lookup"><span data-stu-id="27c18-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="27c18-112">In den Ergebnissen können Sie die IP-Adresse für diese Aktivität im Ergebnisbereich anzeigen.</span><span class="sxs-lookup"><span data-stu-id="27c18-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="27c18-113">Wählen Sie den Überwachungseintrag aus, um detaillierte Informationen im Flyout **Details** anzuzeigen (beispielsweise Client, Benutzer, der eine Aktion ausgeführt hat, usw.).</span><span class="sxs-lookup"><span data-stu-id="27c18-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="27c18-114">Weitere Informationen finden Sie unter [Suchen der IP-Adresse des Computers, der für den Zugriff auf ein kompromittiertes Konto verwendet](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)wurde.</span><span class="sxs-lookup"><span data-stu-id="27c18-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
