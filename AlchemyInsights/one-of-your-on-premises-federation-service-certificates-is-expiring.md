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
ms.openlocfilehash: e1afad0bab317af0f60a6ebda8c3ec8be398e38d
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753029"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Eines Ihrer lokalen Verbunddienst Zertifikate läuft ab

Führen Sie die folgenden Schritte aus, um dieses Problem zu beheben:
  
- Installieren Sie das Microsoft Azure Active Directory-Modul für Windows PowerShell auf dem Computer (wenn das Modul noch nicht installiert ist). Navigieren Sie dazu zu [Azure Active Directory PowerShell für Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Führen Sie die Schritte im Abschnitt "Szenario 1: das AD FS-Token-signierendes Zertifikat ist abgelaufen" des Abschnitts ["Fehler beim Zugriff auf die Website" von AD FS aus, wenn sich ein Verbundbenutzer bei Office 365, Azure oder InTune anmeldet](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Führen Sie die Schritte in t so[aktualisieren oder reparieren Sie die Einstellungen einer Verbunddomäne in Office 365, Azure oder InTune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)aus.
    
Weitere Informationen zum Erneuern von Verbund Zertifikaten finden Sie unter [Certificate Renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

