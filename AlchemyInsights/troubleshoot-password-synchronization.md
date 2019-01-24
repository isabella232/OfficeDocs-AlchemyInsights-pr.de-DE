---
title: Problembehandlung bei kennwortsynchronisierung
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29469994"
---
# <a name="troubleshoot-password-synchronization"></a>Problembehandlung bei kennwortsynchronisierung

Zum Behandeln von Problemen, wenn keine Kennwörter mit Azure AD-Connect Version 1.1.614.0 synchronisiert oder höher sind:
  
1. Öffnen Sie eine neue Windows PowerShell-Sitzung auf dem Server Azure AD-Verbinden mit der Option **als Administrator ausführen** . 
    
2. Führen Sie **Set-ExecutionPolicy RemoteSigned** oder **Set-ExecutionPolicy Unrestricted**. 
    
3. Starten Sie den Assistenten Azure Active Directory verbinden.
    
4. Navigieren Sie zu der ** zusätzliche Aufgaben ** Seite auf ** Troubleshoot **, und klicken Sie auf **Weiter**. 
    
5. Klicken Sie auf der Seite Problembehandlung auf in PowerShell im Menü **Start um die Problembehandlung zu starten** . 
    
6. Wählen Sie im Hauptmenü **Kennwortsynchronisierung behandeln**. 
    
7. Wählen Sie im Menü Sub **Kennwortsynchronisierung funktioniert nicht in allen**. 
    
 **Verstehen der Ergebnisse des Vorgangs zur Problembehandlung**
  
Der Problembehandlung Task führt die folgenden überprüft:
  
- Überprüft, dass das Synchronisierungsfeature Kennwort für Ihren Azure AD-Mandanten aktiviert ist.
    
- Überprüft, dass der Azure AD-Connect-Server nicht ist in der staging-Modus.
    
- Für jeden vorhandenen lokalen Active Directory Connector (der vorhandenen Active Directory-Gesamtstruktur entspricht):
    
- 
  - Überprüft, dass die Funktion "Kennwort Synchronisierung" aktiviert ist.
    
  - Sucht nach Kennwort Synchronisierung Heartbeat-Ereignisse in der Windows-Anwendungsereignisprotokolle.
    
  - Für jede Active Directory-Domäne unter der lokalen Active Directory-Verbindung:
    
  - Überprüft, ob die Domäne aus dem Azure AD-Connect Server erreichbar ist.
    
  - Überprüft, dass die Active Directory-Domänendienste (AD DS)-Konten, die von der lokalen Active Directory-Verbindung verwendet wurde, die richtige Benutzername, Kennwort und erforderliche Berechtigungen für die Synchronisierung von Kennwörtern.
    
Weitere Hilfe zur Problembehandlung für Kennwort Sync finden Sie unter [Troubleshoot kennwortsynchronisierung mit Azure AD-Connect-Synchronisierung](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  

