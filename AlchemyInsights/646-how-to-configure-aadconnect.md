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
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28289232"
---
# <a name="configure-sync-features"></a>Konfigurieren von Sync-features

Azure Active Directory verbinden gehören verschiedene Features, die standardmäßig aktiviert sind, oder Sie können später aktivieren. Einige Features erfordern eine zusätzliche Konfiguration in bestimmten Umgebungen.
  
- [Filtern](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) Grenzwerte für die Objekte werden in Azure Active Directory synchronisiert. Computerkonten werden vom Standard, alle Benutzer, Kontakte, Gruppen und Windows 10 synchronisiert. Sie können ein- oder Ausschließen von Objekten, die basierend auf Domänen, Organisationseinheiten oder andere Attribute. 
    
- [Kennwort Hash Synchronisierung](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronisiert den Hashwert des Kennworts aus der lokalen Active Directory Azure AD. Auf diese Weise können die kennwortverwaltung an einem Standort, aber Verwendung desselben Kennworts in beiden lokalen und cloud-Umgebungen. Da Active Directory die autoritative Quelle ist, können Sie Ihre eigene Kennwortrichtlinien. 
    
- [Self-service-Kennwort zurücksetzen (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) können Benutzer ihre eigenen Kennwörter in der Cloud beim Anwenden von Ihrer lokalen Kennwortrichtlinie weiterhin zurücksetzen. 
    
- [Gerät Rückschreiben](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) ermöglicht registrierte Geräten in Azure AD wieder im lokalen Active Directory geschrieben werden, damit sie für bedingten Zugriff verwendet werden können. 
    
- [Verhindern von unbeabsichtigten löscht](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) ist standardmäßig aktiviert, um zu verhindern, dass zu viele gleichzeitige objektlöschungen (mehr als 500 Objekte pro Synchronisierung). Sie können diese Einstellung, um die Anforderungen Ihrer Organisation ändern. 
    
- [Automatische Aktualisierung](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) ist standardmäßig für express-Installationen aktiviert und können Sie sicherstellen, dass Ihre Version von Azure Active Directory verbinden immer aktuell ist. 
    

