---
title: 902 (Synchronisierungsfehler aufgrund doppelter Objekte)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 06cd582c30a59a94ee117728bd5daebecca77bc8
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757994"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Synchronisierungsfehler aufgrund doppelter Objekte

Wenn die Verzeichnissynchronisierung abgeschlossen ist, wird möglicherweise eine der folgenden Fehlermeldungen angezeigt:

- Dieses Objekt kann in Microsoft Online Services nicht aktualisiert werden, da die folgenden Attribute, die mit diesem Objekt verknüpft sind, Werte enthalten, die möglicherweise bereits einem anderen Objekt in Ihrem lokalen Verzeichnis zugeordnet sind.

- In Ihrem Microsoft Online Services-Verzeichnis ist bereits ein synchronisiertes Objekt mit derselben Proxyadresse vorhanden.

- Dieses Objekt kann nicht aktualisiert werden, da die folgenden Attribute, die mit diesem Objekt verknüpft sind, Werte enthalten, die möglicherweise bereits einem anderen Objekt in Ihren lokalen Verzeichnisdiensten zugeordnet sind: userPrincipalName.

Um das Problem zu identifizieren und zu beheben, laden Sie das [IdFix Dirsync-Tool zur Fehlerbehebung](https://www.microsoft.com/download/details.aspx?id=36832)herunter, und führen Sie es aus.

Weitere Informationen finden Sie unter [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
