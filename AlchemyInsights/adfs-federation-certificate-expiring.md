---
title: Ablauf des ADFS-Verbundzertifikats
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
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821950"
---
# <a name="adfs-federation-certificate-expiring"></a>Ablauf des ADFS-Verbundzertifikats

Führen Sie die folgenden Schritte aus, um dieses Problem zu beheben:
  
1. Installieren Sie das Microsoft Azure Active Directory-Modul für Windows PowerShell auf dem Computer (wenn das Modul noch nicht installiert ist). Wechseln Sie dazu zu [Verwalten von Azure AD mithilfe Windows PowerShell](https://aka.ms/aadposh).

2. Führen Sie die Schritte im Abschnitt "Szenario 1: Das AD FS-Tokensignaturzertifikat ist abgelaufen" des Fehlers "Es gab ein Problem beim Zugriff auf die Website" von AD FS aus, wenn sich ein Verbundbenutzer bei [Microsoft 365, Azure](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)oder Intune einschreibt.

3. Führen Sie die Schritte unter Aktualisieren oder Reparieren der Einstellungen einer [Verbunddomäne in Microsoft, Azure oder Intune aus.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Weitere Informationen zum Verlängern von Verbundzertifikaten finden Sie unter [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
