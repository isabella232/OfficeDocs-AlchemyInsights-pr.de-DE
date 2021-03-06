---
title: Konfigurieren des Bereitstellungsdiensts
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
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480749"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="2eb59-102">Konfigurieren des Bereitstellungsdiensts</span><span class="sxs-lookup"><span data-stu-id="2eb59-102">Configuring the Provision service</span></span>

<span data-ttu-id="2eb59-103">Damit die automatisierte Benutzerbereitstellung funktioniert, benötigt Azure AD gültige Anmeldeinformationen, mit denen eine Verbindung mit der Workday Web Services-API hergestellt werden kann.</span><span class="sxs-lookup"><span data-stu-id="2eb59-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="2eb59-104">Darüber hinaus überprüft die Schaltfläche Verbindung testen in der App Workday to AD User Provisioning auch, ob sie eine Verbindung mit dem Azure AD Connect Provisioning Agent herstellen kann, der der AD-Domäne zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="2eb59-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="2eb59-105">Wenn das Azure-Portal beim Speichern der Anmeldeinformationen einen Fehler zurücksennt, führen Sie die folgenden empfohlenen Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="2eb59-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="2eb59-106">Vergewissern Sie sich, dass Sie das Benutzerkonto für das Workday Integration System konfiguriert haben, wie im Lernprogrammabschnitt Konfigurieren des [Integrationssystembenutzers in Workday angegeben.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="2eb59-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="2eb59-107">Vergewissern Sie sich, dass der Azure AD Connect Provisioning Agent Service auf Ihrem lokalen Windows-Server mit der Dienstverwaltungskonsole ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="2eb59-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="2eb59-108">Sie können auch den Status des Agents im Azure-Portal überprüfen, indem Sie auf die Schaltfläche Lokale Agents anzeigen klicken.</span><span class="sxs-lookup"><span data-stu-id="2eb59-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="2eb59-109">Stellen Sie sicher, dass Sie den Wert für das Feld "Workday Username" mit dem Format username@workday-tenant-name eingeben.</span><span class="sxs-lookup"><span data-stu-id="2eb59-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="2eb59-110">Wenn der Name des workday-tenant-name fehlt, schlägt die Workday-Authentifizierung fehl.</span><span class="sxs-lookup"><span data-stu-id="2eb59-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="2eb59-111">Wenn Sie die Integration mit dem Workday-Implementierungs-Mandanten konfigurieren, notieren Sie sich die geplanten Ausfallzeiten ihres Workday-Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2eb59-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="2eb59-112">Workday hat die Ausfallzeit für seine Implementierungs-Mandanten an Wochenenden (in der Regel von Freitagabend bis Samstagvormittag) geplant, und Konnektivitätsfehler während dieses Ausfallzeitfensters sind ein bekanntes Problem, das automatisch behoben wird, sobald die Implementierungs-Mandanten wieder online sind.</span><span class="sxs-lookup"><span data-stu-id="2eb59-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="2eb59-113">In seltenen Fällen wird dieser Fehler möglicherweise auch angezeigt, wenn das Kennwort des Integrationssystembenutzers aufgrund der Mandantenaktualisierung geändert wurde oder das Konto gesperrt oder abgelaufen ist.</span><span class="sxs-lookup"><span data-stu-id="2eb59-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="2eb59-114">Überprüfen Sie den Status des Integrationssystembenutzers bei Ihrem Workday-Administrator.</span><span class="sxs-lookup"><span data-stu-id="2eb59-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="2eb59-115">Weitere Details zum Konfigurieren von Workday für die automatische Bereitstellung finden Sie unter [Tutorial: Konfigurieren von Workday für die automatische Benutzerbereitstellung](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="2eb59-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
