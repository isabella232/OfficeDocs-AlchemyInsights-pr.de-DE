---
title: Benachrichtigung AAD Connect
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897720"
---
# <a name="notification-aad-connect"></a>Benachrichtigung AAD Connect

- Stellen Sie sicher, dass Sie autorisiert sind, den Vorgang durchzuführen. Globale Administratoren haben standardmäßig Zugriff. Darüber hinaus können Sie die rollenbasierte [Zugriffssteuerung verwenden,](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) um die Registrierungsberechtigung an den Mitwirkenden zu delegieren.
- Stellen Sie sicher, dass die erforderlichen Endpunkte aktiviert und aufgrund der Firewall nicht blockiert werden. Weitere Informationen finden Sie unter [Requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Die Registrierung kann fehlschlagen, da ausgehende Kommunikation von der Netzwerkschicht einer SSL-Überprüfung unterzogen wird.
- Stellen Sie sicher, dass Sie die Benachrichtigungseinstellungen für Azure AD Connect Health überprüft haben, und überprüfen Sie Ihre Einstellung. Informationen zum Konfigurieren der Benachrichtigungseinstellungen für Azure AD Connect Health-Benachrichtigungen finden Sie in diesem [Handbuch](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).
- Weitere Informationen zum AAD Connect Health-Synchronisierungsbericht und zum Herunterladen finden Sie unter [Synchronisierungsbericht auf Objektebene.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Informationen zur Problembehandlung bei AAD Connect-Integritätswarnungen finden Sie im Handbuch zur Problembehandlung für [AAD Connect Integritätswarnungen](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) und häufig gestellte Fragen unter [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
