---
title: Probleme mit der Administrator zustimmung
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49888302"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="b7bf7-102">Probleme mit der Administrator zustimmung</span><span class="sxs-lookup"><span data-stu-id="b7bf7-102">Admin consent issues</span></span>

1. <span data-ttu-id="b7bf7-103">Aktivieren Sie den [Workflow für die Administratorgenehmigung,](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) damit Benutzer die Administratorgenehmigung direkt über den Zustimmungsbildschirm anfordern können.</span><span class="sxs-lookup"><span data-stu-id="b7bf7-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="b7bf7-104">Wenn während des Zustimmungsprozesses unerwartete Fehler angezeigt werden, finden Sie in diesem Artikel Informationen zur Problembehandlung: Unerwarteter Fehler bei der Zustimmung zu [einer Anwendung.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)</span><span class="sxs-lookup"><span data-stu-id="b7bf7-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="b7bf7-105">Erfahren Sie mehr über die Administrator-Zustimmung [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) auf der [Microsoft Identity Platform,](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)wie die Zustimmungsaufforderung funktioniert und wie Sie eine Anforderung für die [mandantenweite Administrator zustimmung auswerten.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="b7bf7-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="b7bf7-106">Anwendungen, die in die Microsoft Identity Platform integriert werden, folgen einem Autorisierungsmodell, mit dem Benutzer und Administratoren steuern können, wie auf Daten zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="b7bf7-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="b7bf7-107">Die Implementierung des Autorisierungsmodells wurde auf dem Microsoft Identity Platform-Endpunkt aktualisiert und ändert, wie eine App mit der Microsoft Identity Platform interagieren muss.</span><span class="sxs-lookup"><span data-stu-id="b7bf7-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="b7bf7-108">Eine Übersicht über dieses Autorisierungsmodell, einschließlich Bereiche, Berechtigungen und Zustimmung, finden Sie unter "Berechtigungen und Zustimmung" im [Microsoft Identity](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) Platform-Endpunkt.</span><span class="sxs-lookup"><span data-stu-id="b7bf7-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>