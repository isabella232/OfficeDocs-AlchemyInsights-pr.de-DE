---
title: Nicht angezeigte Vertraulichkeits Bezeichnungen
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 72dc88a55b55954f34c95fa5b5038f472261c5bb
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758429"
---
# <a name="sensitivity-labels-not-appearing"></a>Nicht angezeigte Vertraulichkeits Bezeichnungen

Mithilfe von Sensitivitäts Bezeichnungen können Sie Ihren vertraulichen Inhalt klassifizieren und schützen. Sie können im Microsoft 365 Compliance Center, im Microsoft 365 Security Center oder im Sicherheits & Compliance Center von Microsoft 365 unter Klassifizierung > Sensitivitäts Bezeichnungen erstellt werden. Weitere Informationen zu dieser Funktion finden Sie unter [Overview of Sensitivity Labels](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).

Wenn Sie Ihre Vertraulichkeits Bezeichnungen konfiguriert haben, diese aber nicht in den Office-Apps angezeigt werden, überprüfen Sie Folgendes:

- Vergewissern Sie sich, dass die Vertraulichkeits Bezeichnung für die gewünschten Benutzer und Gruppen [veröffentlicht](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) wurde.

- Vergewissern Sie sich, dass der Benutzer eine APP verwendet, die Sensitivitäts Bezeichnungen unterstützt – siehe [Sensitivitäts Bezeichnungen in Ihrem Dokument](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Wenn Sie [Azure Information Protection-Bezeichnungen migrieren](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), sollten Sie die [hier](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)aufgelisteten Überlegungen beachten.

- Unterstützung von Datenverlustprävention (DLP): Derzeit können nur Aufbewahrungs Bezeichnungen als Bedingung in DLP-Richtlinien verwendet werden.  Die Unterstützung von Sensitivitäts Bezeichnungen in einer DLP-Richtlinie ist noch nicht verfügbar, aber wir arbeiten daran.

- Wenn die Verschlüsselung für eine Vertraulichkeits Bezeichnung aktiviert ist, können Sie Folgendes auswählen:
    - Berechtigungen sofort zuweisen
    - Benutzern die Zuweisung von Berechtigungen überlassen


Weitere Informationen zu möglichen Problemen finden Sie unter [bekannte Probleme mit Sensitivitäts Bezeichnungen](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).