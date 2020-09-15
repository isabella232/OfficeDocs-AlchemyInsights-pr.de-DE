---
title: Active Directory nicht synchronisiert
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697628"
---
# <a name="active-directory-not-syncing"></a>Active Directory nicht synchronisiert

Wenn Sie Synchronisierungsfehler wie "keine neuere Synchronisierung" oder den Status "Verzeichnissynchronisierung" im Office-Verwaltungsportal erhalten, sagt "Zuletzt synchronisiert vor mehr als 3 Tagen", kann es sein, dass AADConnect falsche Einstellungen oder unzureichende Berechtigungen zum Ausführen einer Synchronisierung besitzt.  

Durch die Neuinstallation von AADConnect mithilfe von Express-Einstellungen kann das Problem schnell behoben werden:

1. [Laden Sie die neueste Version von AADConnect herunter](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Befolgen Sie die Anweisungen für die Express Installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Weitere Informationen zu AADConnect-Dienstkonten finden Sie unter [Azure AD Connect: Konten und Berechtigungen](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
