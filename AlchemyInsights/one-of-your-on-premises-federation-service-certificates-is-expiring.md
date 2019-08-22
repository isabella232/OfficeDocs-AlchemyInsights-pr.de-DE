---
title: Eines Ihrer lokalen Verbunddienst Zertifikate läuft ab
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
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 00cbc77cb178d59a3115e44874a16f506e4408c6
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543564"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Eines Ihrer lokalen Verbunddienst Zertifikate läuft ab

Führen Sie die folgenden Schritte aus, um dieses Problem zu beheben:
  
- Installieren Sie das Microsoft Azure Active Directory Modul für Windows PowerShell auf dem Computer (falls das Modul noch nicht installiert ist). Wechseln Sie dazu zu [Azure Active Directory PowerShell for Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Befolgen Sie die Schritte im Abschnitt "Szenario 1: abgelaufenes AD FS-Token-Signierungszertifikat" unter ["Fehler beim Zugriff auf die Website" von AD FS, wenn sich ein Verbundbenutzer bei Office 365, Azure oder InTune anmeldet](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Befolgen Sie die Schritte in t[So aktualisieren oder reparieren Sie die Einstellungen einer Verbunddomäne in Office 365, Azure oder InTune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Weitere Informationen zum Erneuern von Verbund Zertifikaten finden Sie unter [Zertifikaterneuerung für O365 und Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

