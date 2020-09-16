---
title: 902 (Synchronisierungsfehler aufgrund doppelter Objekte)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737340"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Synchronisierungsfehler aufgrund doppelter Objekte

Wenn die Verzeichnissynchronisierung in Microsoft 365 abgeschlossen ist, wird möglicherweise eine der folgenden Fehlermeldungen angezeigt:

- Dieses Objekt kann in Microsoft Online Services nicht aktualisiert werden, da die folgenden Attribute, die mit diesem Objekt verknüpft sind, Werte enthalten, die möglicherweise bereits einem anderen Objekt in Ihrem lokalen Verzeichnis zugeordnet sind.

- In Ihrem Microsoft Online Services-Verzeichnis ist bereits ein synchronisiertes Objekt mit derselben Proxyadresse vorhanden.

- Dieses Objekt kann nicht aktualisiert werden, da die folgenden Attribute, die mit diesem Objekt verknüpft sind, Werte enthalten, die möglicherweise bereits einem anderen Objekt in Ihren lokalen Verzeichnisdiensten zugeordnet sind: userPrincipalName.

Um das Problem zu identifizieren und zu beheben, laden Sie das [IdFix Dirsync-Tool zur Fehlerbehebung](https://www.microsoft.com/download/details.aspx?id=36832)herunter, und führen Sie es aus.

Weitere Informationen finden Sie unter [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
