---
title: Problem mit AAD Connect Health
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50453293"
---
# <a name="problem-with-aad-connect-health"></a>Problem mit AAD Connect Health

- Stellen Sie sicher, dass Sie autorisiert sind, den Vorgang durchzuführen. Globale Administratoren haben standardmäßig Zugriff. Darüber hinaus können Sie die rollenbasierte [Zugriffssteuerung verwenden,](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) um die Registrierungsberechtigung an den Mitwirkenden zu delegieren.
- Stellen Sie sicher, dass die erforderlichen Endpunkte aktiviert und aufgrund der Firewall nicht blockiert werden. Weitere Informationen finden Sie unter [Requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Die Registrierung kann fehlschlagen, da ausgehende Kommunikation von der Netzwerkschicht einer SSL-Überprüfung unterzogen wird.
- Stellen Sie sicher, dass Sie die Benachrichtigungseinstellungen für Azure AD Connect Health überprüft haben. Überprüfen Sie ihre Einstellung. In [diesem Handbuch](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) erfahren Sie, wie Sie die Benachrichtigungseinstellungen für Azure AD Connect-Integritätsbenachrichtigungen konfigurieren.
- Weitere Informationen zum AAD Connect Health-Synchronisierungsbericht und zum Herunterladen finden Sie unter [Synchronisierungsbericht auf Objektebene.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Zur Problembehandlung bei AAD Connect Health-Warnungen folgen Sie dem Problembehandlungshandbuch für [AAD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) Integritätsdaten-Warnungen und häufig gestellte Fragen unter [Common AAD Connect Health installations questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
