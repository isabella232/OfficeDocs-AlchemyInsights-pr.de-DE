---
title: 646 zum Konfigurieren von AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: e4ba295cd0661c3454180dd6a15895123840389e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499669"
---
# <a name="configure-sync-features"></a><span data-ttu-id="578ef-102">Konfigurieren von Sync-features</span><span class="sxs-lookup"><span data-stu-id="578ef-102">Configure sync features</span></span>

<span data-ttu-id="578ef-p101">Azure Active Directory verbinden gehören verschiedene Features, die standardmäßig aktiviert sind, oder Sie können später aktivieren. Einige Features erfordern eine zusätzliche Konfiguration in bestimmten Umgebungen.</span><span class="sxs-lookup"><span data-stu-id="578ef-p101">Azure AD Connect includes several features that are enabled by default, or that you can enable later. Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="578ef-p102">[Filtern](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) Grenzwerte für die Objekte werden in Azure Active Directory synchronisiert. Computerkonten werden vom Standard, alle Benutzer, Kontakte, Gruppen und Windows 10 synchronisiert. Sie können ein- oder Ausschließen von Objekten, die basierend auf Domänen, Organisationseinheiten oder andere Attribute.</span><span class="sxs-lookup"><span data-stu-id="578ef-p102">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD. By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized. You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="578ef-p103">[Kennwort Hash Synchronisierung](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronisiert den Hashwert des Kennworts aus der lokalen Active Directory Azure AD. Auf diese Weise können die kennwortverwaltung an einem Standort, aber Verwendung desselben Kennworts in beiden lokalen und cloud-Umgebungen. Da Active Directory die autoritative Quelle ist, können Sie Ihre eigene Kennwortrichtlinien.</span><span class="sxs-lookup"><span data-stu-id="578ef-p103">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD. This allows password management in one location, but use of the same password in both on-premises and cloud environments. Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="578ef-111">[Self-service-Kennwort zurücksetzen (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) können Benutzer ihre eigenen Kennwörter in der Cloud beim Anwenden von Ihrer lokalen Kennwortrichtlinie weiterhin zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="578ef-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="578ef-112">[Gerät Rückschreiben](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) ermöglicht registrierte Geräten in Azure AD wieder im lokalen Active Directory geschrieben werden, damit sie für bedingten Zugriff verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="578ef-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="578ef-p104">[Verhindern von unbeabsichtigten löscht](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) ist standardmäßig aktiviert, um zu verhindern, dass zu viele gleichzeitige objektlöschungen (mehr als 500 Objekte pro Synchronisierung). Sie können diese Einstellung, um die Anforderungen Ihrer Organisation ändern.</span><span class="sxs-lookup"><span data-stu-id="578ef-p104">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization). You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="578ef-115">[Automatische Aktualisierung](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) ist standardmäßig für express-Installationen aktiviert und können Sie sicherstellen, dass Ihre Version von Azure Active Directory verbinden immer aktuell ist.</span><span class="sxs-lookup"><span data-stu-id="578ef-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

