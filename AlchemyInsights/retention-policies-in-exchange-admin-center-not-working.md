---
title: Aufbewahrungsrichtlinien im Exchange Admin Center funktionieren nicht
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952227"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Aufbewahrungsrichtlinien im Exchange Admin Center

Wenn sie möchten, dass wir automatisierte Prüfungen für die unten genannten Einstellungen ausführen, wählen Sie die Schaltfläche "Zurück" <- oben auf dieser Seite aus, und geben Sie dann die E-Mail-Adresse des Benutzers ein, der Probleme mit Aufbewahrungsrichtlinien hat.

Wenn Sie Probleme mit Aufbewahrungsrichtlinien im Exchange Admin Center haben, die nicht auf Postfächer oder Elemente angewendet werden, die nicht in das Archivpostfach verschoben werden, überprüfen Sie Folgendes:

**Stammursachen:**

- **Der Assistent für verwaltete** Ordner hat das Postfach des Benutzers nicht verarbeitet. Der Assistent für verwaltete Ordner versucht, jedes Postfach in Ihrer cloudbasierten Organisation einmal alle sieben Tage zu verarbeiten.

  **Lösung:** Führen Sie den Assistenten für verwaltete Ordner aus.

- **RetentionHold** wurde **für das** Postfach aktiviert. Wenn das Postfach in einem Aufbewahrungsspeicher platziert wurde, wird die Aufbewahrungsrichtlinie für das Postfach während dieser Zeit nicht verarbeitet.

  **Lösung:** Überprüfen Sie den Status der Aufbewahrungsaufbewahrungseinstellung und aktualisieren Sie nach Bedarf. Weitere Informationen finden Sie unter [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
 
**Hinweis:** Wenn ein Postfach kleiner als 10 MB ist, wird das Postfach vom Assistenten für verwaltete Ordner nicht automatisch verarbeiten.
 
Weitere Informationen zu Aufbewahrungsrichtlinien im Exchange Admin Center finden Sie unter:

- [Aufbewahrungstags und Aufbewahrungsrichtlinien](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Anwenden einer Aufbewahrungsrichtlinie auf Postfächer oder](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) Hinzufügen oder Entfernen [von Aufbewahrungstags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Identifizieren des auf ein Postfach angewandten Aufbewahrungstyps](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
