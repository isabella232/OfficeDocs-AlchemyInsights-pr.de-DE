---
title: Active Directory wird nicht synchronisiert
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822850"
---
# <a name="active-directory-not-syncing"></a>Active Directory wird nicht synchronisiert

Wenn Sie Synchronisierungsfehler erhalten, z. B. "keine aktuelle Synchronisierung", oder beachten Sie den Verzeichnissynchronisierungsstatus im Office-Verwaltungsportal: "Letzte Synchronisierung vor mehr als 3 Tagen", kann es sein, dass AADConnect falsche Einstellungen oder unzureichende Berechtigungen zum Ausführen einer Synchronisierung hat.  

Durch das erneute Installieren von AADConnect mithilfe von Expresseinstellungen kann das Problem schnell behoben werden:

1. [Laden Sie die neueste Version von AADConnect herunter.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Befolgen Sie die Anweisungen für die Expressinstallation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Weitere Informationen zu AADConnect-Dienstkonten finden Sie unter [Azure AD Connect: Konten und Berechtigungen](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
