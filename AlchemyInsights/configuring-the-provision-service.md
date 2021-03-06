---
title: Konfigurieren des Bereitstellungsdiensts
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480749"
---
# <a name="configuring-the-provision-service"></a>Konfigurieren des Bereitstellungsdiensts

Damit die automatisierte Benutzerbereitstellung funktioniert, benötigt Azure AD gültige Anmeldeinformationen, mit denen eine Verbindung mit der Workday Web Services-API hergestellt werden kann. Darüber hinaus überprüft die Schaltfläche Verbindung testen in der App Workday to AD User Provisioning auch, ob sie eine Verbindung mit dem Azure AD Connect Provisioning Agent herstellen kann, der der AD-Domäne zugeordnet ist.

Wenn das Azure-Portal beim Speichern der Anmeldeinformationen einen Fehler zurücksennt, führen Sie die folgenden empfohlenen Schritte aus:

1. Vergewissern Sie sich, dass Sie das Benutzerkonto für das Workday Integration System konfiguriert haben, wie im Lernprogrammabschnitt Konfigurieren des [Integrationssystembenutzers in Workday angegeben.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Vergewissern Sie sich, dass der Azure AD Connect Provisioning Agent Service auf Ihrem lokalen Windows-Server mit der Dienstverwaltungskonsole ausgeführt wird. Sie können auch den Status des Agents im Azure-Portal überprüfen, indem Sie auf die Schaltfläche Lokale Agents anzeigen klicken.
3. Stellen Sie sicher, dass Sie den Wert für das Feld "Workday Username" mit dem Format username@workday-tenant-name eingeben. Wenn der Name des workday-tenant-name fehlt, schlägt die Workday-Authentifizierung fehl.
4. Wenn Sie die Integration mit dem Workday-Implementierungs-Mandanten konfigurieren, notieren Sie sich die geplanten Ausfallzeiten ihres Workday-Mandanten. Workday hat die Ausfallzeit für seine Implementierungs-Mandanten an Wochenenden (in der Regel von Freitagabend bis Samstagvormittag) geplant, und Konnektivitätsfehler während dieses Ausfallzeitfensters sind ein bekanntes Problem, das automatisch behoben wird, sobald die Implementierungs-Mandanten wieder online sind.
5. In seltenen Fällen wird dieser Fehler möglicherweise auch angezeigt, wenn das Kennwort des Integrationssystembenutzers aufgrund der Mandantenaktualisierung geändert wurde oder das Konto gesperrt oder abgelaufen ist. Überprüfen Sie den Status des Integrationssystembenutzers bei Ihrem Workday-Administrator.

Weitere Details zum Konfigurieren von Workday für die automatische Bereitstellung finden Sie unter [Tutorial: Konfigurieren von Workday für die automatische Benutzerbereitstellung](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
