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
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 2b0a1527ab1b16f56a97891445a2dcb4570302f5
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533806"
---
# <a name="troubleshoot-password-synchronization"></a>Problembehandlung bei der Kennwortsynchronisierung

Zur Behandlung von Problemen, bei denen keine Kennwörter mit Azure AD Connect-Version 1.1.614.0 oder höher synchronisiert werden:
  
1. Öffnen Sie eine neue Windows PowerShell Sitzung auf Ihrem Azure AD Connect-Server mit der Option **als Administrator ausführen** .

2. Führen Sie " **ExecutionPolicy RemoteSigned** " oder " **festgelegt-ExecutionPolicy Unrestricted**" aus.

3. Starten Sie den Azure AD Connect-Assistenten.

4. Navigieren Sie zur Seite **Weitere Aufgaben** , wählen Sie **Problembehandlung**aus, und klicken Sie auf **weiter**.

5. Klicken Sie auf der Seite Problembehandlung auf **starten, um das Menü Problembehandlung in PowerShell zu starten** .

6. Wählen Sie im Hauptmenü die Option **Problembehandlung für die Kennwortsynchronisierung**aus.

7. Wählen Sie im Untermenü die Option **Kennwortsynchronisierung funktioniert überhaupt nicht**aus.

**Grundlegendes zu den Ergebnissen der Aufgaben zur Problembehandlung**
  
Die Problem Behandlungs Aufgabe führt die folgenden Prüfungen durch:
  
- Überprüft, ob das Feature für die Kennwortsynchronisierung für den Azure AD Mandanten aktiviert ist.

- Überprüft, ob sich der Azure AD Connect-Server nicht im stagingmodus befindet.

- Für jeden vorhandenen lokalen Active Directory Connector (der einer vorhandenen Active Directory Gesamtstruktur entspricht):

- 
  - Überprüft, ob das Feature für die Kennwortsynchronisierung aktiviert ist.

  - Sucht nach Kenn Wort Synchronisierungs Takt Ereignissen in den Windows-Anwendungsereignisprotokollen.

  - Für jede Active Directory Domäne unter dem lokalen Active Directory Connector:

  - Überprüft, ob die Domäne über den Azure AD Connect-Server erreichbar ist.

  - Überprüft, ob die vom lokalen Active Directory Connector verwendeten Active Directory-Domänendienste Konten (AD DS) über den korrekten Benutzernamen, das Kennwort und die erforderlichen Berechtigungen für die Kennwortsynchronisierung verfügen.

Weitere Hilfe zur Problembehandlung bei der Kennwortsynchronisierung finden Sie unter [Problembehandlung bei der Kennwortsynchronisierung mit Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  