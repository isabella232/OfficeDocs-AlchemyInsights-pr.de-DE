---
title: Bedingte Zugriff mit Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 3b50bc96a879017b62e42e1849f72e68408a0d9d
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662326"
---
# <a name="conditional-access-with-intune"></a>Bedingte Zugriff mit Intune

Verwenden von **Bedingten Zugriff** mit Intune sind 3 Schritte erforderlich: 
  
- Erstellen Sie eine **Bedingte Zugriffsrichtlinie** , die definiert, welche Ressourcen geschützt sind und welche Bedingungen müssen erfüllt sein, um diese Ressourcen zuzugreifen. Vor dem Zugriff auf Unternehmens-e-Mail-muss beispielsweise ein Gerät kompatibel sein. 
    
- Erstellen einer **Compliance-Richtlinien** , um Einstellungen zu definieren, die erfüllt sein müssen, bevor das Gerät kompatibel ist. Beispielsweise muss ein Gerät eine PIN-Nummer der mindestens 6 Stellen aufweisen, bevor kompatibel ist. 
    
- Sicherstellen, dass **Kompatibilitätsrichtlinien** und **Bedingte Zugriffsrichtlinien** geplant, um die gewünschten Benutzergruppen. Dies erfordert möglicherweise bestimmte Gruppen von Benutzern in Azure Active Directory erstellen. 
    
Weitere Informationen:
  
- [Bedingte Access bewährte Methoden](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Erste Schritte mit bedingten Zugriff](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

