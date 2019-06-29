---
title: 646 Konfigurieren von AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 0569cb10c1d1dd422709de5d2569e43ee9d75386
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35385337"
---
# <a name="configure-sync-features"></a>Konfigurieren von Synchronisierungsfeatures

Azure AD Connect umfasst mehrere Features, die standardmäßig aktiviert sind oder die Sie später aktivieren können. Einige Features erfordern zusätzliche Konfigurationen in bestimmten Umgebungen.

- [Filter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) Grenzwerte die Objekte werden mit Azure AD synchronisiert. Standardmäßig werden alle Computerkonten "Benutzer", "Kontakte", "Gruppen" und "Windows 10" synchronisiert. Sie können Objekte basierend auf Domänen, OUs oder anderen Attributen einschließen oder ausschließen.

- Bei der [Kennworthash Synchronisierung](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) wird der Kennworthash vom lokalen Active Directory auf Azure AD synchronisiert. Dadurch wird die Kennwortverwaltung an einem Ort ermöglicht, jedoch wird das gleiche Kennwort sowohl in lokalen als auch in Cloud-Umgebungen verwendet. Da Active Directory die autorisierende Quelle ist, können Sie Ihre eigenen Kennwortrichtlinien verwenden.

- [Self-Service Password Reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) ermöglicht Benutzern das Zurücksetzen Ihrer eigenen Kennwörter in der Cloud, während Ihre lokale Kennwortrichtlinie weiterhin angewendet wird.

- Durch das [Geräte](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) Rückschreiben können registrierte Geräte in Azure AD in das lokale Active Directory zurückgeschrieben werden, damit Sie für bedingten Zugriff verwendet werden können.

- [Verhindern](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) Sie, dass versehentliche Löschungen standardmäßig aktiviert sind, um zu viele gleichzeitige Objektlöschungen zu verhindern (mehr als 500 Objekte pro Synchronisierung). Sie können diese Einstellung so ändern, dass Sie den Anforderungen Ihrer Organisation entspricht.

- Das [Automatische Upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) ist für Express-Installationen standardmäßig aktiviert und stellt sicher, dass Ihre Version von Azure AD Connect immer aktuell ist.
