---
title: Eine von Ihrer lokalen Dienst Verbundzertifikaten läuft ab
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
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 89a4dd910d43d70e849be19d5f88e281f6d19834
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29469800"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Eine von Ihrer lokalen Dienst Verbundzertifikaten läuft ab

Gehen Sie folgendermaßen vor, um dieses Problem zu beheben:
  
- Installieren Sie die Microsoft Azure Active Directory-Modul für Windows PowerShell auf dem Computer (sofern das Modul nicht bereits installiert ist). Wechseln Sie zu diesem Zweck zu [Azure Active Directory PowerShell für Diagramm](https://docs.microsoft.com/en-us/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Führen Sie die Schritte in der "Szenario 1: die AD FS Tokensignaturzertifikat abgelaufen" im Abschnitt ["Ist ein Problem aufgetreten, den Zugriff auf die Website" Fehler von AD FS, wenn ein Verbundbenutzer bei Office 365, Azure, oder Intune anmeldet](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Führen Sie die Schritte[zum Aktualisieren oder reparieren die Einstellungen einer verbunddomäne in Office 365, Azure, oder Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)int.
    
Weitere Informationen zum Erneuern von Zertifikaten für den Verbund finden Sie unter [Erneuerung von Zertifikaten für Office 365 und Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

