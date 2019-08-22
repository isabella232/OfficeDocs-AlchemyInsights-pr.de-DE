---
title: Bedingter Zugriff mit InTune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504993"
---
# <a name="conditional-access-with-intune"></a>Bedingter Zugriff mit InTune

Die Verwendung von **bedingtem Zugriff** mit InTune erfordert 3 Schritte: 
  
- Erstellen Sie eine **Richtlinie für den bedingten Zugriff** , die definiert, welche Ressourcen geschützt werden, und welche Bedingungen erfüllt sein müssen, um auf diese Ressourcen zuzugreifen. Beispielsweise muss ein Gerät kompatibel sein, bevor auf Firmen-e-Mails zugegriffen werden kann. 
    
- Erstellen Sie eine **Konformitätsrichtlinie** , um Einstellungen zu definieren, die erfüllt sein müssen, bevor das Gerät als konform betrachtet wird. Ein Gerät muss beispielsweise eine PIN von mindestens 6 Ziffern aufweisen, bevor es als konform gilt. 
    
- Sicherstellen, dass sowohl **Compliance-Richt** Linien als auch **Richtlinien für bedingten Zugriff** auf die gewünschten Benutzergruppen zugeschnitten sind. Dies erfordert möglicherweise das Erstellen bestimmter Benutzergruppen in Azure Active Directory. 
    
Weitere Informationen:
  
- [Bewährte Methoden für bedingten Zugriff](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Erste Schritte mit bedingtem Zugriff](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

