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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708061"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Synchronisierungsfehler aufgrund doppelter Objekte

Möglicherweise erhalten Sie eine der folgenden Fehlermeldungen, wenn die Verzeichnissynchronisierung in Microsoft 365 abgeschlossen ist:

- Dieses Objekt kann nicht Microsoft Online Services aktualisiert werden, da die folgenden diesem Objekt zugeordneten Attribute Werte aufweisen, die möglicherweise bereits einem anderen Objekt im lokalen Verzeichnis zugeordnet sind.

- Ein synchronisiertes Objekt mit derselben Proxyadresse ist bereits in Ihrem Microsoft Online Services vorhanden.

- Dieses Objekt kann nicht aktualisiert werden, da die folgenden Diesem Objekt zugeordneten Attribute Werte aufweisen, die möglicherweise bereits einem anderen Objekt in Ihren lokalen Verzeichnisdiensten zugeordnet sind: UserPrincipalName.

Laden Sie das [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix)herunter, und führen Sie es aus, um das Problem zu identifizieren und zu beheben.

Weitere Informationen finden Sie unter [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
