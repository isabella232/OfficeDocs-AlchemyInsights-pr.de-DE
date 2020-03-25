---
title: DLP benötigt möglicherweise einen benutzerdefinierten Typ
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932657"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP benötigt möglicherweise einen benutzerdefinierten Typ

**Wichtig**: viele SharePoint Online-und OneDrive-Kunden führen geschäftskritische Anwendungen für den Dienst aus, der im Hintergrund ausgeführt wird. Dazu gehören Inhaltsmigration, Verhinderung von Datenverlusten (Data Loss Prevention, DLP) und Sicherungslösungen. In diesen noch nie dagewesenen Zeiten machen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online- und OneDrive-Dienste für Ihre Benutzer, die von dem Dienst in Remotearbeitsszenarien mehr denn je abhängig sind, weiterhin hochgradig verfügbar und zuverlässig sind.

Zur Unterstützung dieses Ziels haben wir strengere Drosselungsgrenzen für Hintergrundanwendungen (Migration, DLP und Sicherungslösungen) während der Tageszeit unter der Woche eingeführt. Sie sollten davon ausgehen, dass diese Apps in diesen Zeiten einen sehr begrenzten Durchsatz erreichen. Während der Abendstunden und an Wochenenden wird der Dienst für die Region jedoch in der Lage sein, ein erheblich höheres Volumen an Anforderungen von Hintergrundanwendungen zu verarbeiten.

**DLP erfordert möglicherweise einen benutzerdefinierten Informationstyp.**

Mit einer Richtlinie zur Verhinderung von Datenverlust (Data Loss Prevention, DLP) können Sie vertrauliche Daten in Ihrer Organisation identifizieren und schützen. In einigen Szenarien müssen Sie möglicherweise einen eigenen **benutzerdefinierten** Typ für vertrauliche Informationen erstellen, um die Daten Ihrer Organisation zu schützen.

Beispielsweise kann es sein, dass Ihre Organisation Mitarbeiter-IDs oder andere Daten in einem bestimmten für Ihre org spezifischen Format identifizieren und schützen muss. Wenn dies der Fall ist, finden Sie weitere Informationen in den folgenden Artikeln.
  
 **Anpassen eines benutzerdefinierten vertraulichen Informationstyps**
  
Wenn ein integrierter vertraulicher Informationstyp Ihren Anforderungen mit nur wenigen Optimierungen entspricht, können Sie [einen integrierten vertraulichen Informationstyp anpassen](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type). Beispielsweise können Sie Stichwörter hinzufügen oder entfernen oder unterstützende Beweise wie ein Datum oder eine Adresse hinzufügen oder entfernen.
  
 **Erstellen eines benutzerdefinierten vertraulichen Informationstyps**
  
Wenn Sie jedoch einen anderen Typ vertraulicher Informationen insgesamt identifizieren und schützen müssen, können Sie [einen benutzerdefinierten Typ vertraulicher Informationen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) auf der Benutzeroberfläche des Security & Compliance Center erstellen.
  
**Erstellen eines benutzerdefinierten Typs für vertrauliche Informationen in Security & Compliance Center PowerShell**

Wenn die Benutzeroberfläche nicht alle benötigten Optionen bereitstellt, können Sie [in Security & Compliance Center PowerShell einen benutzerdefinierten Typ für vertrauliche Informationen erstellen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell). Wenn Sie mit einer XML-Datei beginnen, können Sie jede verfügbare Option verwenden.
