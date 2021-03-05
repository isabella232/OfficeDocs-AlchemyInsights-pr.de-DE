---
title: Problem mit einem einzelnen Benutzer
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
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428690"
---
# <a name="problem-with-single-user"></a>Problem mit einem einzelnen Benutzer

- Der Benutzer wurde möglicherweise nicht bereitgestellt, da der Dienst noch keine Möglichkeit hatte, den Benutzer auszuwerten. Lesen Sie die Anleitungen für die Dauer der Bereitstellung sowie die Statusleiste auf der Seite Bereitstellungskonfiguration. Wenn der im Abschnitt zusätzliche Details angegebene stabile Zustand vor dem Datum liegt, an dem der Benutzer erstellt/aktualisiert/gelöscht wurde, bedeutet dies, dass der Benutzer noch nicht ausgewertet wurde. In diesem Szenario sollten Sie am besten warten, bis der Bereitstellungsdienst abgeschlossen ist.

  - Beachten Sie, dass unser Dienst nur Änderungen an einem Benutzer im Quellsystem (Cloud HR) kennt. Es muss eine gültige Änderung im Quellsystem für Azure AD vorhanden sein, um die Änderung zu erkennen und in Active Directory zu fließen.
- Der Bereitstellungsdienst hat den Benutzer ausgewertet und festgestellt, dass er nicht bereitgestellt werden sollte:
  - Wenn Sie einen attributbasierten Scopingfilter festgelegt haben, stellen Sie sicher, dass der Benutzer die angegebenen Kriterien erfüllt.
  - Wenn bereits Benutzer im Zielsystem und der Status des Benutzers in der Quell- und Ziel übereinstimmung vorhanden sind, werden wir keine weiteren Maßnahmen ergreifen.
- Der Bereitstellungsdienst hat versucht, den Benutzer zu bereitstellen, und es ist ein Fehler fehlgeschlagen. Überprüfen Sie für diese Szenarien die Registerkarte Problembehandlung und Empfehlungen der Bereitstellungsprotokolle:
  - Ein erforderliches Attribut für den Benutzer fehlt möglicherweise in lokalem Active Directory oder Azure AD. Beispielsweise generieren die Generierungsregeln userPrincipalName oder sAMAccountName nicht den richtigen Wert.
  - Das übereinstimmende Attribut (in der Regel employeeId) wird nicht für einen eindeutigen Benutzer in lokalem Active Directory oder Azure AD aufgelöst. Beispielsweise gibt es zwei Benutzer mit der gleichen employeeId in AD, und der Dienst gibt einen Fehlercode zurück, der doppelte Zieleinträge für denselben Quelleintrag angibt.

Informationen zum Überprüfen von Protokollen für einzelne Benutzer und Gruppen finden Sie unter Überprüfen der Bereitstellungsprotokolle auf ein Problem [mit einem bestimmten Benutzer.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
