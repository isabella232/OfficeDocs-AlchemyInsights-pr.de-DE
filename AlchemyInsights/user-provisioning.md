---
title: Benutzerbereitstellung
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
- "9004348"
- "8428"
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430748"
---
# <a name="user-provisioning"></a>Benutzerbereitstellung

- Verwenden Sie [die On-Demand-Bereitstellungsfunktion,](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) um einen Benutzer zur Verfügung zu stellen und detaillierte Diagnosen zu den schritten zu erhalten.
- Informationen zur Behebung von Problemen bei der Bereitstellung von Benutzern und Gruppen finden Sie im Fehlerbehebungshandbuch [Es werden keine Benutzer bereitgestellt](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned).
- Wenn Sie feststellen, dass Benutzer nicht bereitgestellt werden, lesen Sie [Bereitstellungsprotokolle (Vorschau)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) in Azure Active Directory (AD). Suchen Sie nach Protokolleinträgen, die sich auf einen bestimmten Benutzer beziehen.
- Starten Sie die Bereitstellung regelmäßig neu, um alle Benutzer zu fangen, die in einem vorherigen Bereitstellungszyklus verpasst wurden.
- Der Benutzer/die Gruppe wurde möglicherweise nicht bereitgestellt, da unser Dienst noch keine Möglichkeit hatte, den Benutzer auszuwerten. Lesen Sie die Anleitungen für die Dauer der Bereitstellung sowie die Statusleiste auf der Seite Bereitstellungskonfiguration. Wenn der im Abschnitt zusätzliche Details angegebene stabile Zustand vor dem Datum liegt, an dem der Benutzer erstellt/aktualisiert/gelöscht wurde, bedeutet dies, dass der Benutzer noch nicht ausgewertet wurde. In diesem Szenario sollten Sie am besten warten, bis der Bereitstellungsdienst abgeschlossen ist. Wenn der stabile Zustand erreicht wurde, wird empfohlen, einen Neustart von der Benutzeroberfläche im Azure-Portal aus zu starten.
  - Beachten Sie, dass unser Dienst nur Änderungen an einem Benutzer/einer Gruppe im Quellsystem (Azure Active Directory) kennt. Wenn ein Benutzer/eine Gruppe direkt in der Anwendung entfernt wird (z. B. ServiceNow), sind wir uns dieser Änderungen nicht bewusst und nehmen kein Rollback basierend auf dem Status des Benutzers im Quellsystem vor. In diesem Szenario ist es am besten, ein Rollback der Änderung direkt in der Zielanwendung zu starten.
- Unser Dienst hat den Benutzer/die Gruppe ausgewertet und festgestellt, dass er nicht bereitgestellt werden sollte:
  - Wenn Sie den Bereich auf zugewiesene Benutzer und Gruppen festgelegt haben, überprüfen Sie, ob der Benutzer/die Gruppe der Anwendung zugewiesen ist.
  - Wenn der Benutzer/die Gruppe der Anwendung zugewiesen ist, stellen Sie sicher, dass sie nicht der Standardzugriffsrolle zugewiesen sind. Diese Rolle kann nicht für die Bereitstellung verwendet werden.
  - Wenn Sie einen attributbasierten Scopingfilter festgelegt haben, stellen Sie sicher, dass der Benutzer die angegebenen Kriterien erfüllt.
  - Wenn bereits Benutzer im Zielsystem und der Status des Benutzers in der Quell- und Ziel übereinstimmung vorhanden sind, werden wir keine weiteren Maßnahmen ergreifen.
- Unser Dienst hat versucht, den Benutzer zu bereitstellen, und es ist ein Fehler fehlgeschlagen. Überprüfen Sie für diese Szenarien die Registerkarte Problembehandlung und Empfehlungen der Bereitstellungsprotokolle:
  - Ein erforderliches Attribut für den Benutzer fehlt möglicherweise in Azure Active Directory oder nicht mit dem von der Drittanbieteranwendung benötigten Format. Beispielsweise kann das Country-Attribut für einen Benutzer auf USA festgelegt werden, wenn es us sein sollte.
  - Das Attribut ist ein referenzielles Attribut, das noch nicht in der Zielanwendung vorhanden ist. Ein referenzielles Attribut ist ein Attribut, das auf ein anderes Objekt verweist, z. B. auf einen Benutzer, der Mitglied einer Gruppe ist. Die BENUTZER-ID befindet sich im Memberattribut der Gruppe, kann jedoch nur verarbeitet werden, wenn das Benutzerobjekt, auf das sie verweist, bereits vorhanden ist.
