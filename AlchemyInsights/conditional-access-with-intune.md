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
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393540"
---
# <a name="conditional-access-with-intune"></a>Bedingter Zugriff mit InTune

Die Verwendung des **bedingten Zugriffs** mit InTune erfordert drei Schritte: 
  
- Erstellen Sie eine **Richtlinie für den bedingten Zugriff** , die definiert, welche Ressourcen geschützt werden, und welche Bedingungen erfüllt sein müssen, um auf diese Ressourcen zugreifen zu können. Ein Gerät muss beispielsweise vor dem Zugriff auf geschäftliche e-Mails kompatibel sein. 
    
- Erstellen Sie eine **Konformitätsrichtlinie** , um Einstellungen zu definieren, die erfüllt sein müssen, bevor das Gerät als kompatibel eingestuft wird. Ein Gerät muss beispielsweise über eine PIN von mindestens 6 Ziffern verfügen, bevor es als kompatibel angesehen wird. 
    
- Sicherstellen, dass sowohl **Konformitätsrichtlinien** als auch **Richtlinien für den bedingten Zugriff** für die gewünschten Benutzergruppen vorgesehen sind. Dies erfordert möglicherweise das Erstellen bestimmter Benutzergruppen in Azure Active Directory. 
    
Weitere Informationen:
  
- [Bewährte Methoden für bedingten Zugriff](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Erste Schritte mit bedingtem Zugriff](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

