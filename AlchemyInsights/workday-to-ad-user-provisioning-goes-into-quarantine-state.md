---
title: Workday zu AD-Benutzerbereitstellung wechselt in den Quarantänezustand
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
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430745"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="2ca00-102">Workday zu AD-Benutzerbereitstellung wechselt in den Quarantänezustand</span><span class="sxs-lookup"><span data-stu-id="2ca00-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="2ca00-103">**Workday zu AD-Benutzerbereitstellung wechselt in den Quarantänezustand, und es werden keine Benutzer in AD erstellt**</span><span class="sxs-lookup"><span data-stu-id="2ca00-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="2ca00-104">Der Auftrag „Workday zu AD-Benutzerbereitstellung“ ist in den Quarantänezustand gewechselt, und die Überwachungsprotokolle zeigen Exportfehlerereignisse mit der Fehlermeldung **Fehler: OperationsError-SvcErr: Ein Betriebsfehler ist aufgetreten. Es wurde kein übergeordneter Verweis für den Verzeichnisdienst konfiguriert. Der Verzeichnisdienst ist daher nicht in der Lage, Verweise auf Objekte außerhalb dieser Gesamtstruktur zu erstellen.**.</span><span class="sxs-lookup"><span data-stu-id="2ca00-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="2ca00-105">Dieser Fehler tritt in der Regel auf, wenn die Organisationseinheit des Active Directory-Containers nicht korrekt eingestellt ist oder wenn es Probleme mit der für **parentDistinguishedName** verwendeten Ausdruckszuordnung gibt.</span><span class="sxs-lookup"><span data-stu-id="2ca00-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="2ca00-106">Überprüfen Sie die Standardorganisationseinheit für den Parameter **Neue Benutzer** auf Tippfehler.</span><span class="sxs-lookup"><span data-stu-id="2ca00-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="2ca00-107">Stellen Sie sicher, dass die angegebene Organisationseinheit bereits in Ihrem AD existiert.</span><span class="sxs-lookup"><span data-stu-id="2ca00-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="2ca00-108">Wenn Sie das **parentDistinguishedName**-Objekt in der Attributzuordnung verwenden, stellen Sie sicher, dass es immer in einen bekannten Container innerhalb der AD-Domäne ausgewertet wird.</span><span class="sxs-lookup"><span data-stu-id="2ca00-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="2ca00-109">Prüfen Sie das Exportereignis in den Überwachungsprotokollen, um den erzeugten Wert anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="2ca00-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="2ca00-110">Weitere Details zum Konfigurieren von Workday für die automatische Bereitstellung finden Sie unter [Tutorial: Konfigurieren von Workday für die automatische Benutzerbereitstellung](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="2ca00-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

