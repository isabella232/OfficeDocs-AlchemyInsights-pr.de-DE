---
title: Problem mit einem einzelnen Benutzer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428690"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="62b7f-102">Problem mit einem einzelnen Benutzer</span><span class="sxs-lookup"><span data-stu-id="62b7f-102">Problem with single user</span></span>

- <span data-ttu-id="62b7f-103">Der Benutzer wurde möglicherweise nicht bereitgestellt, da der Dienst noch keine Möglichkeit hatte, den Benutzer auszuwerten.</span><span class="sxs-lookup"><span data-stu-id="62b7f-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="62b7f-104">Lesen Sie die Anleitungen für die Dauer der Bereitstellung sowie die Statusleiste auf der Seite Bereitstellungskonfiguration.</span><span class="sxs-lookup"><span data-stu-id="62b7f-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="62b7f-105">Wenn der im Abschnitt zusätzliche Details angegebene stabile Zustand vor dem Datum liegt, an dem der Benutzer erstellt/aktualisiert/gelöscht wurde, bedeutet dies, dass der Benutzer noch nicht ausgewertet wurde.</span><span class="sxs-lookup"><span data-stu-id="62b7f-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="62b7f-106">In diesem Szenario sollten Sie am besten warten, bis der Bereitstellungsdienst abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="62b7f-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="62b7f-107">Beachten Sie, dass unser Dienst nur Änderungen an einem Benutzer im Quellsystem (Cloud HR) kennt.</span><span class="sxs-lookup"><span data-stu-id="62b7f-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="62b7f-108">Es muss eine gültige Änderung im Quellsystem für Azure AD vorhanden sein, um die Änderung zu erkennen und in Active Directory zu fließen.</span><span class="sxs-lookup"><span data-stu-id="62b7f-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="62b7f-109">Der Bereitstellungsdienst hat den Benutzer ausgewertet und festgestellt, dass er nicht bereitgestellt werden sollte:</span><span class="sxs-lookup"><span data-stu-id="62b7f-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="62b7f-110">Wenn Sie einen attributbasierten Scopingfilter festgelegt haben, stellen Sie sicher, dass der Benutzer die angegebenen Kriterien erfüllt.</span><span class="sxs-lookup"><span data-stu-id="62b7f-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="62b7f-111">Wenn bereits Benutzer im Zielsystem und der Status des Benutzers in der Quell- und Ziel übereinstimmung vorhanden sind, werden wir keine weiteren Maßnahmen ergreifen.</span><span class="sxs-lookup"><span data-stu-id="62b7f-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="62b7f-112">Der Bereitstellungsdienst hat versucht, den Benutzer zu bereitstellen, und es ist ein Fehler fehlgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="62b7f-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="62b7f-113">Überprüfen Sie für diese Szenarien die Registerkarte Problembehandlung und Empfehlungen der Bereitstellungsprotokolle:</span><span class="sxs-lookup"><span data-stu-id="62b7f-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="62b7f-114">Ein erforderliches Attribut für den Benutzer fehlt möglicherweise in lokalem Active Directory oder Azure AD.</span><span class="sxs-lookup"><span data-stu-id="62b7f-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="62b7f-115">Beispielsweise generieren die Generierungsregeln userPrincipalName oder sAMAccountName nicht den richtigen Wert.</span><span class="sxs-lookup"><span data-stu-id="62b7f-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="62b7f-116">Das übereinstimmende Attribut (in der Regel employeeId) wird nicht für einen eindeutigen Benutzer in lokalem Active Directory oder Azure AD aufgelöst.</span><span class="sxs-lookup"><span data-stu-id="62b7f-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="62b7f-117">Beispielsweise gibt es zwei Benutzer mit der gleichen employeeId in AD, und der Dienst gibt einen Fehlercode zurück, der doppelte Zieleinträge für denselben Quelleintrag angibt.</span><span class="sxs-lookup"><span data-stu-id="62b7f-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="62b7f-118">Informationen zum Überprüfen von Protokollen für einzelne Benutzer und Gruppen finden Sie unter Überprüfen der Bereitstellungsprotokolle auf ein Problem [mit einem bestimmten Benutzer.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)</span><span class="sxs-lookup"><span data-stu-id="62b7f-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
