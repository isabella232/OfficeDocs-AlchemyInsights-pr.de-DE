---
title: Workday zu AD-Benutzerbereitstellung wechselt in den Quarantänezustand
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036491"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Workday zu AD-Benutzerbereitstellung wechselt in den Quarantänezustand

**Workday zu AD-Benutzerbereitstellung wechselt in den Quarantänezustand, und es werden keine Benutzer in AD erstellt**

Der Auftrag „Workday zu AD-Benutzerbereitstellung“ ist in den Quarantänezustand gewechselt, und die Überwachungsprotokolle zeigen Exportfehlerereignisse mit der Fehlermeldung **Fehler: OperationsError-SvcErr: Ein Betriebsfehler ist aufgetreten. Es wurde kein übergeordneter Verweis für den Verzeichnisdienst konfiguriert. Der Verzeichnisdienst ist daher nicht in der Lage, Verweise auf Objekte außerhalb dieser Gesamtstruktur zu erstellen.**. Dieser Fehler tritt in der Regel auf, wenn die Organisationseinheit des Active Directory-Containers nicht korrekt eingestellt ist oder wenn es Probleme mit der für **parentDistinguishedName** verwendeten Ausdruckszuordnung gibt.

Überprüfen Sie die Standardorganisationseinheit für den Parameter **Neue Benutzer** auf Tippfehler. Stellen Sie sicher, dass die angegebene Organisationseinheit bereits in Ihrem AD existiert. Wenn Sie das **parentDistinguishedName**-Objekt in der Attributzuordnung verwenden, stellen Sie sicher, dass es immer in einen bekannten Container innerhalb der AD-Domäne ausgewertet wird. Prüfen Sie das Exportereignis in den Überwachungsprotokollen, um den erzeugten Wert anzuzeigen.

Weitere Details zum Konfigurieren von Workday für die automatische Bereitstellung finden Sie unter [Tutorial: Konfigurieren von Workday für die automatische Benutzerbereitstellung](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).

