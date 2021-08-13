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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 4bfbe6b2dd9a2112f0cb7af0d6e7a46693bc70680895fd674ddb0332b7071797
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53937100"
---
# <a name="active-directory-not-syncing"></a>Active Directory wird nicht synchronisiert

Wenn Sie Synchronisierungsfehler erhalten, z. B. "keine kürzliche Synchronisierung", oder beachten Sie, dass der Status der Verzeichnissynchronisierung im Office Verwaltungsportal besagt: "Letzte Synchronisierung vor mehr als 3 Tagen", kann es sein, dass AADConnect über falsche Einstellungen oder unzureichende Berechtigungen zum Ausführen einer Synchronisierung verfügt.  

Durch erneutes Installieren von AADConnect mithilfe von Expresseinstellungen kann das Problem schnell behoben werden:

1. [Laden Sie die neueste Version von AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771)herunter.

2. [Folgen Sie den Anweisungen für die Expressinstallation.](/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect muss unter Windows Server 2012 oder höher installiert sein. Dieser Server muss der Domäne beigetreten sein und kann ein Domänencontroller oder ein Mitgliedsserver sein. Eine vollständige Liste der Azure AD-Verbinden Anforderungen und Voraussetzungen erhalten Sie unter ["Voraussetzungen für Azure AD Verbinden".](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Weitere Informationen zu AADConnect-Dienstkonten finden Sie unter [Azure AD Connect: Konten und Berechtigungen](/azure/active-directory/hybrid/reference-connect-accounts-permissions).
