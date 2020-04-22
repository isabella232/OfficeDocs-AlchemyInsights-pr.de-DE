---
title: Bedingter Zugriff mit InTune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706020"
---
# <a name="conditional-access-with-intune"></a>Bedingter Zugriff mit InTune

Die Verwendung von **bedingtem Zugriff** mit InTune erfordert 3 Schritte: 
  
- Erstellen Sie eine **Richtlinie für den bedingten Zugriff** , die definiert, welche Ressourcen geschützt werden, und welche Bedingungen erfüllt sein müssen, um auf diese Ressourcen zuzugreifen. Beispielsweise muss ein Gerät kompatibel sein, bevor auf Firmen-e-Mails zugegriffen werden kann. 
    
- Erstellen Sie eine **Konformitätsrichtlinie** , um Einstellungen zu definieren, die erfüllt sein müssen, bevor das Gerät als konform betrachtet wird. Ein Gerät muss beispielsweise eine PIN von mindestens 6 Ziffern aufweisen, bevor es als konform gilt. 
    
- Sicherstellen, dass sowohl **Compliance-Richt** Linien als auch **Richtlinien für bedingten Zugriff** auf die gewünschten Benutzergruppen zugeschnitten sind. Dies erfordert möglicherweise das Erstellen bestimmter Benutzergruppen in Azure Active Directory. 
    
Weitere Informationen:
  
- [Bewährte Methoden für bedingten Zugriff](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Erste Schritte mit bedingtem Zugriff](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

