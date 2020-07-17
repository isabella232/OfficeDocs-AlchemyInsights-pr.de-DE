---
title: Informationen zur Identität in Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146775"
---
# <a name="about-identity-in-yammer"></a>Informationen zur Identität in Yammer

Es wird empfohlen, dass für alle Netzwerke die folgenden Schritte ausgeführt werden, um identitätsbezogene Probleme zu vermeiden:

1. Erzwingen Sie die Office 365-Identität nach der Bereitstellung von Microsoft 365-Konten für Benutzer in Azure AD, um sicherzustellen, dass alle Benutzer sich mit ihrem Microsoft 365-Hauptkonto anmelden. Weitere Informationen finden Sie unter [Erzwingen der Office 365-Identität für Yammer-Benutzer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Konsolidieren Sie mehrerer Yammer-Netzwerke. Älteren Yammer-Konfigurationen erlauben, dass mehrere Yammer-Netzwerke mit einem Mandanten verbunden werden. Weitere Informationen finden Sie unter [Netzwerkmigration: Konsolidieren von mehreren Yammer-Netzwerken](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Optional können Sie eine Lizenz für Yammer erzwingen, um die Verwendung von Yammer für Benutzer ohne Lizenz zu sperren. Weitere Informationen finden Sie unter [Verwalten von Yammer-Benutzerlizenzen in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Überprüfen Sie abschließend die Benutzerliste für ältere Yammer-Netzwerke, und sperren Sie Legacybenutzer. Es wird empfohlen, die Benutzer auszusetzen (zu deaktivieren), statt sie zu löschen, da das Löschen nicht rückgängig gemacht werden kann. Weitere Informationen finden Sie unter [Überwachen von Yammer-Benutzern in mit Office 365 verbundenen Netzwerken](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) und [Entfernen von Benutzern](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Indem Sie Yammer mit diesen Schritten konfigurieren, sind Sie auch bereit, Ihr Yammer Netzwerk für Microsoft 365 für den nativen Modus zu konfigurieren. Weitere Informationen finden Sie unter [Konfigurieren eines Yammer-Netzwerks für den nativen Modus für Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).