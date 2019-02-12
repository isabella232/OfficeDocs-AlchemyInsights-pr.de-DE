---
title: AD FS-Verbund Zertifikat abläuft.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 55529265d2356a911624026107fb639f93e29abd
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29925379"
---
# <a name="adfs-federation-certificate-expiring"></a>AD FS-Verbund Zertifikat abläuft.

Gehen Sie folgendermaßen vor, um dieses Problem zu beheben:
  
1. Installieren Sie die Microsoft Azure Active Directory-Modul für Windows PowerShell auf dem Computer (sofern das Modul nicht bereits installiert ist). Wechseln Sie zu diesem Zweck zum [Verwalten von Azure Active Directory mithilfe von Windows PowerShell](https://aka.ms/aadposh).
    
2. Führen Sie die Schritte in der "Szenario 1: die AD FS Tokensignaturzertifikat abgelaufen" im Abschnitt ["Ist ein Problem aufgetreten, den Zugriff auf die Website" Fehler von AD FS, wenn ein Verbundbenutzer bei Office 365, Azure, oder Intune anmeldet](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
3. Führen Sie die Schritte [zum Aktualisieren oder reparieren die Einstellungen einer verbunddomäne in Office 365, Azure, oder Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
    Weitere Informationen zum Erneuern von Zertifikaten für den Verbund finden Sie unter [Erneuern von Zertifikaten für Office 365 und Azure Active Directory Federation](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
    

