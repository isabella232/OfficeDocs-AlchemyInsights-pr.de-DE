---
title: Nicht angezeigte Vertraulichkeits Bezeichnungen
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801183"
---
# <a name="sensitivity-labels-not-appearing"></a>Nicht angezeigte Vertraulichkeits Bezeichnungen

Mithilfe von Sensitivitäts Bezeichnungen können Sie Ihren vertraulichen Inhalt klassifizieren und schützen. Sie können im Microsoft 365 Compliance Center, im Microsoft 365 Security Center oder im Sicherheits & Compliance Center von Microsoft 365 unter Klassifizierung > Sensitivitäts Bezeichnungen erstellt werden. Weitere Informationen zu dieser Funktion finden Sie unter [Overview of Sensitivity Labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Wenn Sie Ihre Vertraulichkeits Bezeichnungen konfiguriert haben, diese aber nicht in den Microsoft 365-apps angezeigt werden, überprüfen Sie Folgendes:

- Vergewissern Sie sich, dass die Vertraulichkeits Bezeichnung für die gewünschten Benutzer und Gruppen [veröffentlicht](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) wurde.

- Vergewissern Sie sich, dass der Benutzer eine APP verwendet, die Sensitivitäts Bezeichnungen unterstützt – siehe [Sensitivitäts Bezeichnungen in Ihrem Dokument](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Wenn Sie [Azure Information Protection-Bezeichnungen migrieren](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), sollten Sie die [hier](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)aufgelisteten Überlegungen beachten.

- Unterstützung von Datenverlustprävention (DLP): Derzeit können nur Aufbewahrungs Bezeichnungen als Bedingung in DLP-Richtlinien verwendet werden.  Die Unterstützung von Sensitivitäts Bezeichnungen in einer DLP-Richtlinie ist noch nicht verfügbar, aber wir arbeiten daran.

- Wenn die Verschlüsselung für eine Vertraulichkeits Bezeichnung aktiviert ist, können Sie Folgendes auswählen:
    - Berechtigungen sofort zuweisen
    - Benutzern die Zuweisung von Berechtigungen überlassen


Weitere Informationen zu möglichen Problemen finden Sie unter [bekannte Probleme mit Sensitivitäts Bezeichnungen](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).