---
title: Active Directory nicht synchronisiert
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265195"
---
# <a name="active-directory-not-syncing"></a>Active Directory nicht synchronisiert

Wenn Sie Synchronisierungsfehler wie "keine neuere Synchronisierung" oder den Status "Verzeichnissynchronisierung" im Office-Verwaltungsportal erhalten, sagt "Zuletzt synchronisiert vor mehr als 3 Tagen", kann es sein, dass AADConnect falsche Einstellungen oder unzureichende Berechtigungen zum Durchführen einer Synchronisierung.  

Durch die Neuinstallation von AADConnect mithilfe von Express-Einstellungen kann das Problem schnell behoben werden:

1. [Laden Sie die neueste Version von AADConnect herunter](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Befolgen Sie die Anweisungen für die Express Installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Weitere Informationen zu AADConnect-Dienstkonten finden Sie unter [Azure AD Connect: Accounts and Permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
