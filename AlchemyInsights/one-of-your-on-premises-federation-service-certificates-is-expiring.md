---
title: Eines Ihrer lokalen Verbunddienst Zertifikate läuft ab
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: a4c78f3fdbba7786785f31098c9e80e77a165623
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673496"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Eines Ihrer lokalen Verbunddienst Zertifikate läuft ab

Führen Sie die folgenden Schritte aus, um dieses Problem zu beheben:
  
- Installieren Sie das Microsoft Azure Active Directory Modul für Windows PowerShell auf dem Computer (falls das Modul noch nicht installiert ist). Wechseln Sie dazu zu [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Befolgen Sie die Schritte im Abschnitt "Szenario 1: abgelaufenes AD FS-Token-Signierungszertifikat" unter ["Fehler beim Zugriff auf die Website" von AD FS, wenn sich ein Verbundbenutzer bei Microsoft 365, Azure oder InTune anmeldet](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Führen Sie die Schritte unter [aktualisieren oder Reparieren der Einstellungen einer Verbunddomäne in Microsoft 365, Azure oder InTune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)aus.
    
Weitere Informationen zum Erneuern von Verbund Zertifikaten finden Sie unter [Zertifikaterneuerung für O365 und Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

