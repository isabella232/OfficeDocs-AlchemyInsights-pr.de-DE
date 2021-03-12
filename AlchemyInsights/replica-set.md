---
title: Replikatsatz
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50716271"
---
# <a name="replica-set"></a>Replikatsatz

AADDS wird auch als verwaltete Domäne bezeichnet. Es handelt sich tatsächlich um zwei Domänencontroller, die vom Back-End ausgeführt und verwaltet werden. Die beiden DCs umfassen einen Haupt-DC und einen Replikations-DC. Sicherungen in AADDS (verwaltete Domäne) sind ein automatisierter Prozess, der von der Azure-Plattform verwaltet wird. Im Falle eines Problems mit Ihrer verwalteten Domäne kann die Azure-Unterstützung Ihnen bei der Wiederherstellung aus der Sicherung helfen.

Sie erstellen jeden Replikatsatz in einem virtuellen Netzwerk. Jedes virtuelle Netzwerk muss mit jedem anderen virtuellen Netzwerk, das den Replikatsatz einer verwalteten Domäne hostet, peered werden. Diese Konfiguration erstellt eine Gitternetzwerktopologie, die die Verzeichnisreplikation unterstützt. Ein virtuelles Netzwerk kann mehrere Replikatsätze unterstützen, sofern sich jeder Replikatsatz in einem anderen virtuellen Subnetz befindet.

Weitere Informationen zum Replikatsatz finden Sie unter [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
