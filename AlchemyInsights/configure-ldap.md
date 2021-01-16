---
title: Konfigurieren von LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876573"
---
# <a name="configure-ldap"></a>Konfigurieren von LDAP

Gehen Sie zum Konfigurieren von LDAP wie folgt vor:

1. Überprüfen Sie die Integrität Ihrer Domäne im [Azure-Portal.](https://aka.ms/aadds-health)
1. Stellen Sie sicher, dass ein gültiges Azure AD-Abonnement verfügbar ist und Azure AD Domain Services aktiviert wurde.
1. Das zum Aktivieren von sicherem LDAP erforderliche Zertifikat muss von einer vertrauenswürdigen öffentlichen Zertifizierungsstelle oder einem selbst signierten Zertifikat erworben werden.
1. Stellen Sie sicher, dass das Zertifikat den erforderlichen Richtlinien [entspricht.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Ungültiges Zertifikat**
1. Führen Sie zum Erneuern eines Zertifikats die schritte zum Erstellen eines neuen Zertifikats und erneuten Ladens aus: [Konfigurieren von LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Informationen zum Beheben eines bekannten Problems mit secure LDAP alerts in Azure Active directory Domain Services finden Sie unter [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
