---
title: Identifizieren von IP-Adressen und Clients in Überwachungsprotokollen
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 7e30a638de5926aa11b8ae637613a48076d7bdc9
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32416960"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="420e6-102">Identifizieren von IP-Adressen und Clients in Überwachungsprotokollen</span><span class="sxs-lookup"><span data-stu-id="420e6-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="420e6-103">Die IP-Adresse, die einer Aktivität eines Benutzers oder Administrators entspricht, wird in den Überwachungsprotokollen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="420e6-103">The IP address that corresponds to an activity by a user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="420e6-104">Die Clientinformationen werden ebenfalls protokolliert.</span><span class="sxs-lookup"><span data-stu-id="420e6-104">The client information is also logged.</span></span> <span data-ttu-id="420e6-105">Hier sind die Schritte zur Identifizierung solcher Informationen</span><span class="sxs-lookup"><span data-stu-id="420e6-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="420e6-106">Melden Sie sich beim [Office 365 Security _AMP_ Compliance Center](https://protection.office.com/) an.</span><span class="sxs-lookup"><span data-stu-id="420e6-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="420e6-107">Klicken Sie auf **Suchen und Untersuchung** , und wählen Sie **Überwachungsprotokoll Suche**aus.</span><span class="sxs-lookup"><span data-stu-id="420e6-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

   <span data-ttu-id="420e6-108">Wenn Sie an einer bestimmten Aktivität interessiert sind, wählen Sie Sie aus der Liste **Aktivitäten** aus.</span><span class="sxs-lookup"><span data-stu-id="420e6-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="420e6-109">Ist dies nicht der Fall, werden alle Aktivitäten für den ausgewählten Benutzer zurückgegeben (Standardeinstellung).</span><span class="sxs-lookup"><span data-stu-id="420e6-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="420e6-110">**Hinweis**: bestimmte Aktivitäten sind möglicherweise nicht im Menü " **Aktivitäten** " verfügbar; Diese Überwachungselemente werden jedoch zurückgegeben, wenn die Option **Ergebnisse für alle Aktivitäten anzeigen** ausgewählt ist (Standardeinstellung).</span><span class="sxs-lookup"><span data-stu-id="420e6-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="420e6-111">Geben Sie den Benutzernamen im Feld **Benutzer** an, wählen Sie den entsprechenden Datumsbereich für die Aktivität aus, und klicken Sie dann auf **Suchen**.</span><span class="sxs-lookup"><span data-stu-id="420e6-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="420e6-112">In den Ergebnissen wird die IP-Adresse für diese Aktivität im Ergebnisbereich angezeigt.</span><span class="sxs-lookup"><span data-stu-id="420e6-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="420e6-113">Wählen Sie den Überwachungsdatensatz aus, um detaillierte Informationen im **Detail** Flyout anzuzeigen (beispielsweise Client, Benutzer, der die Aktion ausgeführt hat, usw.).</span><span class="sxs-lookup"><span data-stu-id="420e6-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="420e6-114">Weitere Informationen finden Sie unter [Suchen der IP-Adresse des Computers, der für den Zugriff auf ein kompromittiertes Konto verwendet wird](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="420e6-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
