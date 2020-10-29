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
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="9186f-102">InTune-Exchange-lokaler Connector</span><span class="sxs-lookup"><span data-stu-id="9186f-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="9186f-103">Ausführliche Informationen zum Einrichten des Connectors zwischen InTune und Exchange, der lokal gehostet wird, finden Sie in der folgenden Dokumentation:</span><span class="sxs-lookup"><span data-stu-id="9186f-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="9186f-104">Einrichten des lokalen InTune-Exchange-Connectors in Microsoft InTune Azure</span><span class="sxs-lookup"><span data-stu-id="9186f-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="9186f-105">**Häufig gestellte Fragen:**</span><span class="sxs-lookup"><span data-stu-id="9186f-105">**FAQ:**</span></span>

<span data-ttu-id="9186f-106">F: beim Versuch, den Exchange Connector einzurichten, wird ein Fehler wie "die Exchange Connector-Version wird nicht unterstützt" angezeigt.</span><span class="sxs-lookup"><span data-stu-id="9186f-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="9186f-107">Was könnte die Ursache sein?</span><span class="sxs-lookup"><span data-stu-id="9186f-107">What could be the cause?</span></span>

<span data-ttu-id="9186f-108">A: das Konto, das Sie verwenden, ist ordnungsgemäß lizenziert-es muss eine aktive InTune-Lizenz besitzen.</span><span class="sxs-lookup"><span data-stu-id="9186f-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="9186f-109">F.: ist es möglich, mehrere Exchange-Connectors zu haben?</span><span class="sxs-lookup"><span data-stu-id="9186f-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="9186f-110">A.: Sie können nur einen Exchange Connector pro InTune-Mandanten pro Exchange-Organisation einrichten.</span><span class="sxs-lookup"><span data-stu-id="9186f-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="9186f-111">Der Connector kann nur auf einem Server in einer Exchange-Organisation mit mehreren Servern installiert werden.</span><span class="sxs-lookup"><span data-stu-id="9186f-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="9186f-112">Außerdem können Sie keine Connectors für Exchange lokal und Exchange Online in demselben Mandanten konfiguriert haben.</span><span class="sxs-lookup"><span data-stu-id="9186f-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="9186f-113">F.: kann der Connector ein CAS-Array als Verbindung mit Exchange verwenden?</span><span class="sxs-lookup"><span data-stu-id="9186f-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="9186f-114">A: bei der Angabe eines CAS-Arrays handelt es sich nicht um eine unterstützte Konfiguration im Connector-Setup.</span><span class="sxs-lookup"><span data-stu-id="9186f-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="9186f-115">Es sollte nur ein einzelner Server angegeben werden, der in der Connector-Konfigurationsdatei hart codiert ist, die sich in finden lässt.</span><span class="sxs-lookup"><span data-stu-id="9186f-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="9186f-116">Programmieren von Data\Microsoft\Microsoft InTune auf dem lokalen Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="9186f-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="9186f-117">Suchen Sie den folgenden Eintrag ```<ExchangeWebServiceURL />``` , und ersetzen Sie die URL durch den Exchange-Server.</span><span class="sxs-lookup"><span data-stu-id="9186f-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="9186f-118">**Beispiel**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="9186f-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="9186f-119">Weitere Informationen zur Problembehandlung finden Sie in der folgenden Dokumentation: [Problembehandlung beim lokalen InTune-Exchange Connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="9186f-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="9186f-120">**Aktivieren der ausführlichen Protokollierung für den Exchange Connector**</span><span class="sxs-lookup"><span data-stu-id="9186f-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="9186f-121">Öffnen Sie die Exchange Connector-Ablauf Verfolgungs Konfigurationsdatei zur Bearbeitung.</span><span class="sxs-lookup"><span data-stu-id="9186f-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="9186f-122">Die Datei befindet sich unter:%ProgramData%\Microsoft\Windows InTune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="9186f-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="9186f-123">**Beispiel**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="9186f-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="9186f-124">Suchen Sie die TraceSource mit dem folgenden Schlüssel: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="9186f-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="9186f-125">Ändern Sie den Wert des SourceLevel-Knotens von Information ActivityTracing (Standard) in Verbose ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="9186f-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="9186f-126">**Beispiel:**</span><span class="sxs-lookup"><span data-stu-id="9186f-126">**Example:**</span></span>
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
4. <span data-ttu-id="9186f-127">Neustarten des Microsoft InTune-Exchange-Diensts</span><span class="sxs-lookup"><span data-stu-id="9186f-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="9186f-128">Vollständige Synchronisierung im InTune-Portal bis zum Abschluss und ändern Sie dann den XML-Code wieder in "Information ActivityTracing", und starten Sie den Microsoft InTune Exchange-Dienst neu.</span><span class="sxs-lookup"><span data-stu-id="9186f-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="9186f-129">Der Speicherort der Protokolle lautet wie folgt: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="9186f-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>