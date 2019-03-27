---
title: Problembehandlung bei der Kennwortsynchronisierung
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 1320c0fe839337188162824439be6f15f86b6c90
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/22/2019
ms.locfileid: "30767175"
---
# <a name="troubleshoot-password-synchronization"></a>Problembehandlung bei der Kennwortsynchronisierung

Zur Behandlung von Problemen, bei denen keine Kennwörter mit Azure AD Connect-Version 1.1.614.0 oder höher synchronisiert werden:
  
1. Öffnen Sie auf Ihrem Azure AD Connect-Server eine neue Windows PowerShell-Sitzung mit der Option **als Administrator ausführen** . 
    
2. Führen Sie **Set-ExecutionPolicy RemoteSigned** oder **Set-ExecutionPolicy Unrestricted**aus. 
    
3. Starten Sie den Azure AD Connect-Assistenten.
    
4. Navigieren Sie zu der Seite * * zusätzliche Aufgaben * *, wählen Sie * * Problembehandlung * * aus, und klicken Sie auf **weiter**. 
    
5. Klicken Sie auf der Seite Problembehandlung auf **Start, um das Menü Problembehandlung in PowerShell zu starten** . 
    
6. Wählen Sie im Hauptmenü die Option **Problembehandlung für Kennwortsynchronisierung**aus. 
    
7. Wählen Sie im Untermenü die Option **Kennwortsynchronisierung funktioniert nicht**aus. 
    
 **GrundLegendes zu den Ergebnissen der Problem Behandlungs Aufgabe**
  
Die Problem Behandlungs Aufgabe führt die folgenden Prüfungen aus:
  
- Überprüft, ob die Kennwortsynchronisierung für Ihren Azure AD-Mandanten aktiviert ist.
    
- Überprüft, ob sich der Azure AD Connect-Server nicht im stagingmodus befindet.
    
- Für jeden vorhandenen lokalen Active Directory-Connector (der einer vorhandenen Active Directory-Gesamtstruktur entspricht):
    
- 
  - Überprüft, ob die Kennwortsynchronisierung aktiviert ist.
    
  - Sucht in den Ereignisprotokollen der Windows-Anwendung nach Kenn Wort Synchronisierungs Takt Ereignissen.
    
  - Für jede Active Directory-Domäne unter dem lokalen Active Directory-Connector:
    
  - Überprüft, ob die Domäne vom Azure AD Connect-Server erreichbar ist.
    
  - Überprüft, ob die vom lokalen Active Directory Connector verwendeten Active Directory-Domänendienste (AD DS)-Konten über den richtigen Benutzernamen, das richtige Kennwort und die für die Kennwortsynchronisierung erforderlichen Berechtigungen verfügen.
    
Weitere Hilfe bei der Problembehandlung bei der Kennwortsynchronisierung finden Sie unter [Problembehandlung bei der Kennwortsynchronisierung mit Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  

