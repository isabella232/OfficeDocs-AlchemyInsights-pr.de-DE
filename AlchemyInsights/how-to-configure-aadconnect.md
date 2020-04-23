---
title: 646 Konfigurieren von AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722538"
---
# <a name="configure-sync-features"></a><span data-ttu-id="7fbcc-102">Konfigurieren von Synchronisierungsfeatures</span><span class="sxs-lookup"><span data-stu-id="7fbcc-102">Configure sync features</span></span>

<span data-ttu-id="7fbcc-103">Azure AD Connect umfasst mehrere Features, die standardmäßig aktiviert sind oder die Sie später aktivieren können.</span><span class="sxs-lookup"><span data-stu-id="7fbcc-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="7fbcc-104">Einige Features erfordern zusätzliche Konfigurationen in bestimmten Umgebungen.</span><span class="sxs-lookup"><span data-stu-id="7fbcc-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="7fbcc-105">[Filter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) Grenzwerte die Objekte werden mit Azure AD synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="7fbcc-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="7fbcc-106">Standardmäßig werden alle Computerkonten "Benutzer", "Kontakte", "Gruppen" und "Windows 10" synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="7fbcc-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="7fbcc-107">Sie können Objekte basierend auf Domänen, OUs oder anderen Attributen einschließen oder ausschließen.</span><span class="sxs-lookup"><span data-stu-id="7fbcc-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="7fbcc-108">Bei der [Kennworthash Synchronisierung](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) wird der Kennworthash vom lokalen Active Directory auf Azure AD synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="7fbcc-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="7fbcc-109">Dadurch wird die Kennwortverwaltung an einem Ort ermöglicht, jedoch wird das gleiche Kennwort sowohl in lokalen als auch in Cloud-Umgebungen verwendet.</span><span class="sxs-lookup"><span data-stu-id="7fbcc-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="7fbcc-110">Da Active Directory die autorisierende Quelle ist, können Sie Ihre eigenen Kennwortrichtlinien verwenden.</span><span class="sxs-lookup"><span data-stu-id="7fbcc-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="7fbcc-111">[Self-Service Password Reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) ermöglicht Benutzern das Zurücksetzen Ihrer eigenen Kennwörter in der Cloud, während Ihre lokale Kennwortrichtlinie weiterhin angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="7fbcc-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="7fbcc-112">Durch das [Geräte](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) Rückschreiben können registrierte Geräte in Azure AD in das lokale Active Directory zurückgeschrieben werden, damit Sie für bedingten Zugriff verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="7fbcc-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="7fbcc-113">Verhindern Sie, dass [versehentliche Löschungen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) standardmäßig aktiviert sind, um zu viele gleichzeitige Objektlöschungen zu verhindern (mehr als 500 Objekte pro Synchronisierung).</span><span class="sxs-lookup"><span data-stu-id="7fbcc-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="7fbcc-114">Sie können diese Einstellung so ändern, dass Sie den Anforderungen Ihrer Organisation entspricht.</span><span class="sxs-lookup"><span data-stu-id="7fbcc-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="7fbcc-115">Das [Automatische Upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) ist für Express-Installationen standardmäßig aktiviert und stellt sicher, dass Ihre Version von Azure AD Connect immer aktuell ist.</span><span class="sxs-lookup"><span data-stu-id="7fbcc-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
