---
title: InTune-Exchange-lokaler Connector
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791524"
---
# <a name="intune-exchange-on-premise-connector"></a>InTune-Exchange-lokaler Connector

Ausführliche Informationen zum Einrichten des Connectors zwischen InTune und Exchange, der lokal gehostet wird, finden Sie in der folgenden Dokumentation:

[Einrichten des lokalen InTune-Exchange-Connectors in Microsoft InTune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**Häufig gestellte Fragen:**

F: beim Versuch, den Exchange Connector einzurichten, wird ein Fehler wie "die Exchange Connector-Version wird nicht unterstützt" angezeigt. Was könnte die Ursache sein?

A: das Konto, das Sie verwenden, ist ordnungsgemäß lizenziert-es muss eine aktive InTune-Lizenz besitzen.

F.: ist es möglich, mehrere Exchange-Connectors zu haben?

A.: Sie können nur einen Exchange Connector pro InTune-Mandanten pro Exchange-Organisation einrichten. Der Connector kann nur auf einem Server in einer Exchange-Organisation mit mehreren Servern installiert werden.

Außerdem können Sie keine Connectors für Exchange lokal und Exchange Online in demselben Mandanten konfiguriert haben.

F.: kann der Connector ein CAS-Array als Verbindung mit Exchange verwenden?

A: bei der Angabe eines CAS-Arrays handelt es sich nicht um eine unterstützte Konfiguration im Connector-Setup. Es sollte nur ein einzelner Server angegeben werden, der in der Connector-Konfigurationsdatei hart codiert ist, die sich in finden lässt.

Programmieren von Data\Microsoft\Microsoft InTune auf dem lokalen Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml

Suchen Sie den folgenden Eintrag ```<ExchangeWebServiceURL />``` , und ersetzen Sie die URL durch den Exchange-Server.

**Beispiel**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Weitere Informationen zur Problembehandlung finden Sie in der folgenden Dokumentation: [Problembehandlung beim lokalen InTune-Exchange Connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Aktivieren der ausführlichen Protokollierung für den Exchange Connector**

1. Öffnen Sie die Exchange Connector-Ablauf Verfolgungs Konfigurationsdatei zur Bearbeitung.  
Die Datei befindet sich unter:%ProgramData%\Microsoft\Windows InTune Exchange Connector\TracingConfiguration.xml  

**Beispiel**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Suchen Sie die TraceSource mit dem folgenden Schlüssel: OnPremisesExchangeConnectorService  
  
3. Ändern Sie den Wert des SourceLevel-Knotens von Information ActivityTracing (Standard) in Verbose ActivityTracing  

**Beispiel:**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Neustarten des Microsoft InTune-Exchange-Diensts  
5. Vollständige Synchronisierung im InTune-Portal bis zum Abschluss und ändern Sie dann den XML-Code wieder in "Information ActivityTracing", und starten Sie den Microsoft InTune Exchange-Dienst neu.  
6. Der Speicherort der Protokolle lautet wie folgt: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`