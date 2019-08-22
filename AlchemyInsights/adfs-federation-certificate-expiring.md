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
ms.openlocfilehash: c9922258c2d203cc07c1a1055ffa36c23a756115
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36499890"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS-Verbundzertifikat läuft ab

Führen Sie die folgenden Schritte aus, um dieses Problem zu beheben:
  
1. Installieren Sie das Microsoft Azure Active Directory Modul für Windows PowerShell auf dem Computer (falls das Modul noch nicht installiert ist). Wechseln Sie dazu zum [Verwalten von Azure AD mithilfe von Windows PowerShell](https://aka.ms/aadposh).

2. Befolgen Sie die Schritte im Abschnitt "Szenario 1: abgelaufenes AD FS-Token-Signierungszertifikat" unter ["Fehler beim Zugriff auf die Website" von AD FS, wenn sich ein Verbundbenutzer bei Office 365, Azure oder InTune anmeldet](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Führen Sie die Schritte unter [aktualisieren oder Reparieren der Einstellungen einer Verbunddomäne in Office 365, Azure oder InTune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)aus.

    Weitere Informationen zum Erneuern von Verbund Zertifikaten finden Sie unter [Erneuern von Verbund Zertifikaten für Office 365 und Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
