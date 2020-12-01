---
title: Mandant löschen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/30/2020
ms.locfileid: "49477676"
---
# <a name="delete-tenant"></a><span data-ttu-id="37586-102">Mandant löschen</span><span class="sxs-lookup"><span data-stu-id="37586-102">Delete tenant</span></span>

<span data-ttu-id="37586-103">Um eine Azure AD zu löschen, stellen Sie Folgendes sicher:</span><span class="sxs-lookup"><span data-stu-id="37586-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="37586-104">Sie sind ein globaler Administrator für das Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="37586-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="37586-105">Sie sind nicht mit einem Konto angemeldet, das über das Standardverzeichnis wie contoso.onmicrosoft.com im angemeldeten Konto verfügt, beispielsweise admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="37586-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="37586-106">Entfernen Sie alle aktiven Anwendungen in dem Verzeichnis vor dem Löschen.</span><span class="sxs-lookup"><span data-stu-id="37586-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="37586-107">Wenn Sie aktive Anwendungen entfernen möchten, navigieren Sie zu app-Registrierungen, und entfernen Sie die vorhandenen Anwendungen.</span><span class="sxs-lookup"><span data-stu-id="37586-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="37586-108">Es sind keine aktiven Abonnements für Microsoft Online Services vorhanden, wie Microsoft Azure, Office 365 oder Azure AD Premium, die dem Verzeichnis zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="37586-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="37586-109">Übertragen Sie Ihre Abonnements oder beschleunigen Sie die Löschung aktiver Abonnements über Azure-Unterstützung und Abrechnung.</span><span class="sxs-lookup"><span data-stu-id="37586-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="37586-110">Erfahren Sie mehr über das Abbrechen von Office 365-und Azure-Abonnements.</span><span class="sxs-lookup"><span data-stu-id="37586-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="37586-111">Anleitungen zum Zuordnen oder Hinzufügen eines vorhandenen Abonnements zu einem Mandanten finden Sie unter [Associate or Add a Azure Subscription to your Azure AD Mandanten](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="37586-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="37586-112">Es gibt keine aktive Lizenz.</span><span class="sxs-lookup"><span data-stu-id="37586-112">There are no Active license.</span></span> <span data-ttu-id="37586-113">Informationen zum Entfernen von Lizenzen finden Sie unter [Entfernen eines Abonnements zum Entfernen der Lizenz](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="37586-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="37586-114">Es gibt keine anderen aktiven Benutzer im Verzeichnis als den globalen Administrator, wenn Sie versuchen, die Azure AD zu löschen.</span><span class="sxs-lookup"><span data-stu-id="37586-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="37586-115">Entfernen Sie alle anderen aktiven Benutzer, und alle Abhängigkeiten von einem benutzerdefinierten Domänennamen im Mandanten müssen ebenfalls entfernt werden, beispielsweise Benutzer, die mit admin@contoso.com erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="37586-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="37586-116">Ausführlichere Informationen zu den folgenden Schritten:</span><span class="sxs-lookup"><span data-stu-id="37586-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="37586-117">Delete "Azure Active Directory" oder "Subscription" finden Sie unter [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="37586-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="37586-118">Entfernen von Anwendungen im Verzeichnis finden Sie unter [Entfernen von Anwendungen](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="37586-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
