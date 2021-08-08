---
title: IRM-Konfiguration für neue HOME-Funktionen testen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53908971"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>IRM-Konfiguration für neue HOME-Funktionen testen

Um zu überprüfen, ob Ihr Microsoft 365-Mandant für die Verwendung neuer OME-Funktionen konfiguriert ist, führen Sie die folgenden Cmdlets aus, während Sie mit [Exchange Online PowerShell](/powershell/exchange/exchange-online-powershell) verbunden sind:


1. Überprüfen Sie die IRM-Konfiguration Ihres Mandanten, indem Sie `Get-IRMConfiguration` ausführen. Stellen Sie sicher, dass diese Werte auf **True** gesetzt sind:
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Führen Sie mit Ihrer Domain, Absenderadresse und Empfänger `Test-IRMConfiguration` aus. Wenn der Test nicht bestanden wird, untersuchen Sie Ihre IRM-Konfiguration.

Weitere Informationen zum Überprüfen der IRM-Konfiguration finden Sie unter [Überprüfen der neuen OME-Konfiguration in Exchange Online PowerShell](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell).