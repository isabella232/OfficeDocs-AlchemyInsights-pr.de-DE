---
title: ADFS-Verbundzertifikat läuft ab
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: b014e350d5f6f1a61feb223e3d3fd0a1f56f5872
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35357964"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS-Verbundzertifikat läuft ab

Führen Sie die folgenden Schritte aus, um dieses Problem zu beheben:
  
1. Installieren Sie das Microsoft Azure Active Directory Modul für Windows PowerShell auf dem Computer (falls das Modul noch nicht installiert ist). Wechseln Sie dazu zum [Verwalten von Azure AD mithilfe von Windows PowerShell](https://aka.ms/aadposh).

2. Befolgen Sie die Schritte im Abschnitt "Szenario 1: abgelaufenes AD FS-Token-Signierungszertifikat" unter ["Fehler beim Zugriff auf die Website" von AD FS, wenn sich ein Verbundbenutzer bei Office 365, Azure oder InTune anmeldet](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Führen Sie die Schritte unter [aktualisieren oder Reparieren der Einstellungen einer Verbunddomäne in Office 365, Azure oder InTune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)aus.

    Weitere Informationen zum Erneuern von Verbund Zertifikaten finden Sie unter [Erneuern von Verbund Zertifikaten für Office 365 und Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
