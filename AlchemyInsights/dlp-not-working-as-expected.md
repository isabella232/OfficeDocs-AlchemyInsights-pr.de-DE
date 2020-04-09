---
title: DLP funktioniert nicht wie erwartet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: 940169c0edf638b5086d70cc275049f01dcff3cf
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2020
ms.locfileid: "42977437"
---
# <a name="dlp-not-working-as-expected"></a>DLP funktioniert nicht wie erwartet

**Wichtig**: Während dieser beispiellosen Zeiten unternehmen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online und OneDrive-Dienste weiterhin in hohem Ausmaß verfügbar bleiben – Bitte besuchen Sie [SharePoint Online – Temporäre Feature-Anpassungen](https://aka.ms/ODSPAdjustments), um weitere Informationen zu erhalten.

 **Einrichten von DLP**

Haben Sie Probleme mit der **Verhinderung von Datenverlust (DLP)** in Office 365 nicht wie erwartet funktioniert? Wenn dies der Fall ist, stellen Sie sicher, dass Ihre **DLP-Richtlinie** ordnungsgemäß eingerichtet ist und dass Ihre Daten enthalten, wonach die **DLP-Richtlinie** bei der Auswertung sucht.
  
Mit DLP-Richtlinien können Sie vertrauliche Informationen in Ihrer Organisation identifizieren und schützen. Verwenden Sie die Informationen [hier](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp), um DLP-Richtlinien einzurichten.
  
 **Wonach die DLP-Richtlinien suchen**
  
Bei Verwendung der **integrierten Typen für vertrauliche Informationen** im Office 365 Security and Compliance Center suchen DLP-Richtlinien nach bestimmten Mustern und Elementen, wenn diese vertraulichen Typen erkannt werden.
  
- **Integrierte Typen für vertrauliche Informationen**

    Informationen zu den integrierten vertraulichen Typen und was eine DLP-Richtlinie sucht, wenn der vertrauliche Typ erkannt wird, finden Sie unter [was die Typen vertraulicher Informationen suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Benutzerdefinierte Typen für vertrauliche Informationen**

    Wenn Sie versuchen, benutzerdefinierte Typen vertraulicher Informationen zu erstellen, verwenden Sie den folgenden Artikel, um Informationen zum Erstellen eines benutzerdefinierten vertraulichen Typs zu erhalten: [Erstellen eines benutzerdefinierten Typs für vertrauliche Informationen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**Testen einer DLP-Richtlinie**

Wenn Sie Ihre Daten mit einem integrierten oder benutzerdefinierten Typ vertraulicher Informationen testen möchten, verwenden Sie die Option **Testtyp** unter **Klassifikationen** > **vertrauliche Informationstypen**. Weitere Informationen finden Sie unter [Testen benutzerdefinierter vertraulicher Informationstypen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Berichte**
  
- Erhalten Sie vertrauliche Daten Einblicke mit [DLP-Berichten.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Siehe spezifische Details des Ereignisses mit einem [Vorfall Bericht](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).
