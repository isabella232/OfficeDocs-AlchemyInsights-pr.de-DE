---
title: 902 (Synchronisierungsfehler aufgrund doppelter Objekte)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: ce7eeb07cfde16e6d6856a9369c042dcf4f05b63
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420879"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Synchronisierungsfehler aufgrund doppelter Objekte

Wenn die Verzeichnissynchronisierung abgeschlossen ist, wird möglicherweise eine der folgenden Fehlermeldungen angezeigt:

- Dieses Objekt kann in Microsoft Online Services nicht aktualisiert werden, da die folgenden Attribute, die diesem Objekt zugeordnet sind, Werte aufweisen, die möglicherweise bereits einem anderen Objekt in Ihrem lokalen Verzeichnis zugeordnet sind.

- Ein synchronisiertes Objekt mit derselben Proxyadresse ist bereits in Ihrem Microsoft Online Services-Verzeichnis vorhanden.

- Dieses Objekt kann nicht aktualisiert werden, da die folgenden Attribute, die diesem Objekt zugeordnet sind, Werte aufweisen, die möglicherweise bereits einem anderen Objekt in Ihrem lokalen Verzeichnisdienste zugeordnet sind: UserPrincipalName.

Um das Problem zu identifizieren und zu beheben, laden Sie das [IdFix Dirsync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832)herunter und führen es aus.

Weitere Informationen finden Sie unter [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
