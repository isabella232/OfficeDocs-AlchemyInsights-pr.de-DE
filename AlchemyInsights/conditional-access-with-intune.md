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
ms.openlocfilehash: 59f1aefaeec3d655b2388b00e7d58a8c2338504b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28289118"
---
# <a name="conditional-access-with-intune"></a>Bedingte Zugriff mit Intune

Verwenden von **Bedingten Zugriff** mit Intune sind 3 Schritte erforderlich: 
  
- Erstellen Sie eine **Bedingte Zugriffsrichtlinie** , die definiert, welche Ressourcen geschützt sind und welche Bedingungen müssen erfüllt sein, um diese Ressourcen zuzugreifen. Vor dem Zugriff auf Unternehmens-e-Mail-muss beispielsweise ein Gerät kompatibel sein. 
    
- Erstellen einer **Compliance-Richtlinien** , um Einstellungen zu definieren, die erfüllt sein müssen, bevor das Gerät kompatibel ist. Beispielsweise muss ein Gerät eine PIN-Nummer der mindestens 6 Stellen aufweisen, bevor kompatibel ist. 
    
- Sicherstellen, dass **Kompatibilitätsrichtlinien** und **Bedingte Zugriffsrichtlinien** geplant, um die gewünschten Benutzergruppen. Dies erfordert möglicherweise bestimmte Gruppen von Benutzern in Azure Active Directory erstellen. 
    
Weitere Informationen:
  
- [Bedingte Access bewährte Methoden](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/best-practices)
    
- [Erste Schritte mit bedingten Zugriff](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

