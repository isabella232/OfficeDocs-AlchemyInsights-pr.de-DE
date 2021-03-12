---
title: DLP funktioniert nicht wie erwartet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707809"
---
# <a name="dlp-not-working-as-expected"></a>DLP funktioniert nicht wie erwartet

**Wichtig**: Während dieser beispiellosen Zeiten unternehmen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online und OneDrive-Dienste weiterhin in hohem Ausmaß verfügbar bleiben – Bitte besuchen Sie [SharePoint Online – Temporäre Feature-Anpassungen](https://aka.ms/ODSPAdjustments), um weitere Informationen zu erhalten.

 **Einrichten von DLP**

Funktionieren Probleme mit der Verhinderung von Datenverlust **(Data Loss Prevention, DLP)** in Office 365 nicht wie erwartet? Wenn ja, stellen Sie sicher, dass Ihre **DLP-Richtlinie** ordnungsgemäß eingerichtet ist und dass Ihre Daten enthalten, was die **DLP-Richtlinie** bei der Auswertung sucht.
  
Mit DLP-Richtlinien können Sie vertrauliche Informationen in Ihrer Organisation identifizieren und schützen. Verwenden Sie zum Einrichten von DLP-Richtlinien die informationen [hier](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).
  
 **Suchen nach DLP-Richtlinien**
  
Bei der Verwendung der **integrierten** Typen vertraulicher Informationen in den Security and Compliance Centern suchen DLP-Richtlinien nach bestimmten Mustern und Elementen, wenn diese vertraulichen Typen erkannt werden.
  
- **Integrierte Typen vertraulicher Informationen**

    Informationen zu den integrierten Typen "Vertraulich" und zur Suche nach einer DLP-Richtlinie beim Erkennen des Typs "Vertraulich" finden Sie unter: Was die Typen vertraulicher Informationen [suchen.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **Benutzerdefinierte Typen vertraulicher Informationen**

    Wenn Sie versuchen, benutzerdefinierte Typen vertraulicher Informationen zu erstellen, finden Sie im folgenden Artikel Informationen zum Erstellen eines benutzerdefinierten vertraulichen Typs: Erstellen eines benutzerdefinierten [Vertraulichen Informationstyps](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Testen einer DLP-Richtlinie**

Um Ihre Daten mit einem integrierten oder benutzerdefinierten vertraulichen Informationstyp zu testen, verwenden Sie die Option **Testtyp** unter **Klassifizierungen** Vertrauliche  >  **Infotypen**. Weitere Informationen finden Sie unter [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Berichte**
  
- Erhalten Sie Einblicke in vertrauliche Daten mit [DLP-Berichten.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Siehe spezifische Details des Ereignisses mit einem [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
