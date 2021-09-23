---
title: Wechseln von Microsoft-Nameservern zurück zur Verwaltung Ihrer eigenen DNS-Einträge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/22/2021
ms.locfileid: "59481867"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Wechseln von Microsoft-Nameservern zurück zur Verwaltung Ihrer eigenen DNS-Einträge

Sie haben Ihre NS-Einträge zuvor so geändert, dass sie auf Microsoft (ns1.bdm.microsoftonline.com) verweisen, aber sie haben sich jetzt entschieden, Ihre eigenen DNS-Einträge zu verwalten:

Ändern Sie auf der Website Ihrer Domänenregistrierungsstelle den Namenserver wieder in Ihre Registrierungsstelle oder frühere Einstellung. Wenn Sie mit DNS nicht vertraut sind, wenden Sie sich an den Support bei der Domänenregistrierungsstelle. Hinweis: Die Verarbeitung von Änderungen an Nameservern kann manchmal bis zu 48 Stunden dauern. 

1. Wechseln Sie im Microsoft 365 Verwaltungsportal zu **Einstellungen**  >  [**Domänen,**](https://admin.microsoft.com/Adminportal/Home#/Domains)aktivieren Sie das Kontrollkästchen neben der Domäne, und wählen Sie **DNS verwalten** aus. 

2. Wählen Sie im Assistenten Ihre **eigenen DNS-Einträge hinzufügen aus,** und schließen Sie den Assistenten ab. Dies ändert die Art und Weise, wie Ihr DNS verwaltet wird, und ermöglicht es Ihnen dann, die benutzerdefinierten DNS-Einträge hinzuzufügen, die zur Unterstützung der ausgewählten Dienste erforderlich sind.

Wenn Sie Ihre Namenservereinträge in Microsoft geändert haben und über eine Website verfügen, können Sie alternativ DNS-Einträge für die Website hinzufügen, anstatt die Namenserver wieder zu ändern. Weitere Informationen finden Sie unter [Aktualisieren von DNS-Einträgen, um die Website beim aktuellen Hostinganbieter zu belassen](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider).


