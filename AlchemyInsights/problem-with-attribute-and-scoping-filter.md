---
title: Problem mit Attribut- und Bereichsdefinitionsfilter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430751"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="10f17-102">Problem mit Attribut- und Bereichsdefinitionsfilter</span><span class="sxs-lookup"><span data-stu-id="10f17-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="10f17-103">**Problem mit Konflikten zwischen UPN-Werten**</span><span class="sxs-lookup"><span data-stu-id="10f17-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="10f17-104">Die Workday zu AD-Benurtzerbereitstellung zeigt die Fehlermeldung **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique** an.</span><span class="sxs-lookup"><span data-stu-id="10f17-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="10f17-105">Der Vorgang ist fehlgeschlagen, weil der für das Hinzufügen/Ändern angegebene UPN-Wert nicht über die Gesamtstruktur hinweg eindeutig ist.</span><span class="sxs-lookup"><span data-stu-id="10f17-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="10f17-106">Fehlerdetails: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="10f17-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="10f17-107">Der Wert **userPrincipalName**, den der Workday-Connector beim Erstellen des AD-Benutzerkontos festzulegen versucht, existiert in der AD-Zieldomäne bereits.</span><span class="sxs-lookup"><span data-stu-id="10f17-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="10f17-108">Dies bedeutet, dass entweder (1) der Benutzer bereits vorhanden und die Prüfung der entsprechenden ID für den Benutzer fehlgeschlagen ist oder (2) die UPN-Generierungsregel einen Wert generiert hat, der einen Konflikt verursacht.</span><span class="sxs-lookup"><span data-stu-id="10f17-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="10f17-109">Folgende Lösungsschritte werden vorgeschlagen:</span><span class="sxs-lookup"><span data-stu-id="10f17-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="10f17-110">Wenn der Benutzer bereits vorhanden ist und die Prüfung der übereinstimmenden ID das Workday-Konto nicht mit dem Active Directory-Konto verknüpfen konnte, dann prüfen Sie, ob das übereinstimmende ID-Attribut (typischerweise **employeeID**) sowohl in Workday als auch in AD eine exakte Übereinstimmung aufweist.</span><span class="sxs-lookup"><span data-stu-id="10f17-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="10f17-111">Wenn sie nicht übereinstimmen, handelt es sich um ein Datenproblem, das behoben werden muss.</span><span class="sxs-lookup"><span data-stu-id="10f17-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="10f17-112">Wenn der EmployeeID-Wert in Workday beispielsweise 001052 und in AD 1052 lautet, kann das Bereitstellungsmodul die beiden Konten nicht miteinander verknüpfen und versucht, einen Benutzer zu erstellen, der bereits existiert.</span><span class="sxs-lookup"><span data-stu-id="10f17-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="10f17-113">Die Lösung besteht in diesem Fall darin, den **EmployeeID**-Wert in AD so zu ändern, dass er die führenden Nullen enthält und somit 001052 lautet.</span><span class="sxs-lookup"><span data-stu-id="10f17-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="10f17-114">Wenn der die UPN erzeugende Ausdruck keinen eindeutigen Wert generiert, sollten Sie ggf. die Deduplizierungsfunktion **SelectUniqueValue** verwenden, damit jedes Mal ein eindeutiger Wert zu generiert wird.</span><span class="sxs-lookup"><span data-stu-id="10f17-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="10f17-115">**Workday zu AD-Benurtzerbereitstellung legt keinen Manager-Attributwert für AD-Benutzerkonto fest**</span><span class="sxs-lookup"><span data-stu-id="10f17-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="10f17-116">Der Auftrag „Workday zu AD-Benurtzerbereitstellung“ legt den Wert des **manager**-Attributs für AD-Benutzerkonten nicht fest.</span><span class="sxs-lookup"><span data-stu-id="10f17-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="10f17-117">Es gibt zwei mögliche Szenarien, wenn dieses Verhalten auftritt:</span><span class="sxs-lookup"><span data-stu-id="10f17-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="10f17-118">Der Manager in Workday kann nicht in ein entsprechendes AD-Benutzerkonto aufgelöst werden, da der Manager nicht innerhalb der Bereichsdefinition liegt.</span><span class="sxs-lookup"><span data-stu-id="10f17-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="10f17-119">In einem Szenario mit **mehreren AD-Domänen** befindet sich der Manager in Workday nicht in der gleichen Domäne wie der Benutzer.</span><span class="sxs-lookup"><span data-stu-id="10f17-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="10f17-120">Probieren Sie die folgenden Schritte aus, um das Problem zu beheben:</span><span class="sxs-lookup"><span data-stu-id="10f17-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="10f17-121">Wenn Sie Bereichsdefinitionsfilter definiert haben, prüfen Sie zunächst, ob der Manager innerhalb der Bereichsdefinition liegt und die Bereichsdefinitionsklausel erfüllt.</span><span class="sxs-lookup"><span data-stu-id="10f17-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="10f17-122">Wenn der Manager den Bereichsdefinitionsfilter nicht erfüllt, ändern Sie den Filter so, dass der Manager auch innerhalb der Bereichsdefinition des Bereitstellungsvorgangs liegt.</span><span class="sxs-lookup"><span data-stu-id="10f17-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="10f17-123">Wenn Sie über mehrere AD-Domänen verfügen, gilt für den Connector die bekannte Einschränkung, dass er domänenübergreifende Verweise auf Manager nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="10f17-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="10f17-124">Weitere Details zum Konfigurieren von Workday für die automatische Bereitstellung finden Sie unter [Tutorial: Konfigurieren von Workday für die automatische Benutzerbereitstellung](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="10f17-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













