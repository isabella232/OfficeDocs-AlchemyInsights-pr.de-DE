---
title: Ablauf des ADFS-Verbund Zertifikats
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 518261787b1b0df99ee7b3dc3e51dec70e4373bc
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32398339"
---
# <a name="adfs-federation-certificate-expiring"></a>Ablauf des ADFS-Verbund Zertifikats

Führen Sie die folgenden Schritte aus, um dieses Problem zu beheben:
  
1. Installieren Sie das Microsoft Azure Active Directory-Modul für Windows PowerShell auf dem Computer (wenn das Modul noch nicht installiert ist). Gehen Sie dazu zu verwalten von [Azure AD mit Windows PowerShell](https://aka.ms/aadposh).
    
2. Führen Sie die Schritte im Abschnitt "Szenario 1: das AD FS-Token-signierendes Zertifikat ist abgelaufen" des Abschnitts ["Fehler beim Zugriff auf die Website" von AD FS aus, wenn sich ein Verbundbenutzer bei Office 365, Azure oder InTune anmeldet](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
3. Führen Sie die Schritte unter [aktualisieren oder Reparieren der Einstellungen einer Verbunddomäne in Office 365, Azure oder InTune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)aus.
    
    Weitere Informationen zum Erneuern von Verbund Zertifikaten finden Sie unter [Renew Federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
    

