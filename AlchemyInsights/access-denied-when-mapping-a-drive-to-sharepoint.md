---
title: Zugriff verweigert beim Zuordnen eines Laufwerks zu SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 8fc866390d63443c94beef76b6a53a628b85d6d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668742"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a>Beheben von Problemen mit SharePoint-Bibliotheken, die Netzlaufwerken zugeordnet sind

Wenn Sie ein zugeordnetes Netzlaufwerk durchsuchen, wird möglicherweise eine der folgenden Meldungen angezeigt:
  
- **\\Auf Path kann nicht zugegriffen werden. Möglicherweise sind Sie nicht berechtigt, diese Netzwerkressource zu verwenden. Wenden Sie sich an den Administrator dieses Servers, um herauszufinden, ob Sie über Zugriffsberechtigungen verfügen.**

- **Zugriff verweigert. Bevor Sie Dateien an diesem Speicherort öffnen, müssen Sie zunächst die Website der Liste der vertrauenswürdigen Websites hinzufügen, zur Website wechseln und die Option zum automatischen Anmelden auswählen.**

[Erhalten Sie Hilfe bei der Problembehandlung zugeordneter Netzlaufwerke](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).
  
Das Zuordnen einer Bibliothek als Netzlaufwerk ist temporär und wird nur in Internet Explorer unterstützt. Synchronisieren Sie stattdessen [SharePoint-Dateien mit dem neuen OneDrive-synchronisierungsclient](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) , der [Dateien bei Bedarf](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx)enthält. Greifen Sie auf alle Ihre Dateien auf OneDrive zu, ohne lokalen Speicherplatz zu verwenden.
  