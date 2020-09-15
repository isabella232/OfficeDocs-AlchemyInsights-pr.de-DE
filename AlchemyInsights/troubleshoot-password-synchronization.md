---
title: Problembehandlung bei der Kennwortsynchronisierung
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664925"
---
# <a name="troubleshoot-password-synchronization"></a>Problembehandlung bei der Kennwortsynchronisierung

Zur Behandlung von Problemen mit der Kennwortsynchronisierung beginnen Sie mit dieser Aad Connect-Problem Behandlungs Aufgabe, um zu ermitteln, warum Kennwörter nicht synchronisiert werden. Wechseln Sie zunächst zu [Manage Direct Sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Öffnen Sie auf dem Azure AD Connect-Server eine neue Windows PowerShell-Sitzung, und wählen Sie die Option **als Administrator ausführen** aus.

2. Führen Sie "ExecutionPolicy RemoteSigned" oder "festgelegt-ExecutionPolicy Unrestricted" aus.

3. Starten Sie den Azure AD Connect-Assistenten.

4. Wechseln Sie zur Seite Weitere Aufgaben > **Problembehandlung**  >  **als nächstes**.

5. Wählen Sie **Start** aus, um das PowerShell-Problem Behandlungs Menü zu öffnen.

6. Wählen Sie **Problembehandlung bei der Kennwortsynchronisierung**aus.

    Das Problem besteht in der Regel darin, dass ein Kennwort für ein bestimmtes Benutzerkonto nicht synchronisiert ist.

    **Anmerkungen** Die Kennwortsynchronisierung schlägt fehl, wenn die letzte erfolgreiche Kennwortsynchronisierung vor einiger Zeit stattfand.

Weitere Hilfe zur Problembehandlung bei der Kennwortsynchronisierung finden Sie unter [Problembehandlung bei der Kennworthash Synchronisierung mit Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).