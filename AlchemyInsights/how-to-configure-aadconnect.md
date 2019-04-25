---
title: 646 Konfigurieren von AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 44b2532c634bf17d87c562f9506cc1e81cc7e84a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32399770"
---
# <a name="configure-sync-features"></a><span data-ttu-id="6cac2-102">Konfigurieren von Synchronisierungsfeatures</span><span class="sxs-lookup"><span data-stu-id="6cac2-102">Configure sync features</span></span>

<span data-ttu-id="6cac2-103">Azure AD Connect umfasst mehrere Features, die standardmäßig aktiviert sind oder die Sie später aktivieren können.</span><span class="sxs-lookup"><span data-stu-id="6cac2-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="6cac2-104">Einige Features erfordern zusätzliche Konfiguration in bestimmten Umgebungen.</span><span class="sxs-lookup"><span data-stu-id="6cac2-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="6cac2-105">[Filter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) Grenzen die Objekte werden mit Azure AD synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="6cac2-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="6cac2-106">Standardmäßig werden alle Benutzer, Kontakte, Gruppen und Windows 10-Computerkonten synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="6cac2-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="6cac2-107">Sie können Objekte basierend auf Domänen, Organisationseinheiten oder anderen Attributen einschließen oder ausschließen.</span><span class="sxs-lookup"><span data-stu-id="6cac2-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="6cac2-108">[Password Hash Synchronisierung](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronisiert den Kennworthash vom lokalen Active Directory mit Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6cac2-108">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="6cac2-109">Auf diese Weise kann die Kennwortverwaltung an einem Ort, aber in lokalen und Cloud-Umgebungen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="6cac2-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="6cac2-110">Da Active Directory die autorisierende Quelle ist, können Sie Ihre eigenen Kennwortrichtlinien verwenden.</span><span class="sxs-lookup"><span data-stu-id="6cac2-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="6cac2-111">[Self-Service Password Reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) ermöglicht es Benutzern, ihre eigenen Kennwörter in der Cloud zurückzusetzen, während Sie weiterhin Ihre lokale Kennwortrichtlinie anwenden.</span><span class="sxs-lookup"><span data-stu-id="6cac2-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="6cac2-112">[](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) Durch das Rückschreiben von Geräten können registrierte Geräte in Azure AD in das lokale Active Directory zurückgeschrieben werden, damit Sie für bedingten Zugriff verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="6cac2-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="6cac2-113">Verhindern Sie, dass [versehentliche Löschvorgänge](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) standardmäßig aktiviert sind, um zu viele gleichzeitige Objektlöschungen zu verhindern (mehr als 500 Objekte pro Synchronisierung).</span><span class="sxs-lookup"><span data-stu-id="6cac2-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="6cac2-114">Sie können diese Einstellung ändern, um die Anforderungen Ihrer Organisation zu erfüllen.</span><span class="sxs-lookup"><span data-stu-id="6cac2-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="6cac2-115">Das [Automatische Upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) ist für Express Installationen standardmäßig aktiviert und stellt sicher, dass Ihre Version von Azure AD Connect immer aktuell ist.</span><span class="sxs-lookup"><span data-stu-id="6cac2-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
