---
title: Geräterückschreiben
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2021
ms.locfileid: "50255156"
---
# <a name="device-writeback"></a>Geräterückschreiben

Das Rückschreiben von Geräten wird in den folgenden Szenarien verwendet:

- Aktivieren [von Windows Hello for Business mithilfe der Hybridbereitstellung mit Zertifikatvertrauensstellung](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Aktivieren des bedingten Zugriffs auf Basis von Geräten für ADFS (2012 R2 oder höher) geschützte Anwendungen (Vertrauensstellungen der vertrauenden Partei)

    > [!NOTE]
    > Für das Rückschreiben von Geräten ist ein Abonnement für Azure AD Premium erforderlich.

Dies bietet zusätzliche Sicherheit und Sicherheit, dass der Zugriff auf Anwendungen nur vertrauenswürdigen Geräten gewährt wird. Weitere Informationen zum bedingten Zugriff finden Sie unter ["Verwalten](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) von Risiken mit bedingten Zugriff" und einrichten des lokalen bedingten Zugriffs mithilfe der [Azure Active Directory-Geräteregistrierung.](https://docs.microsoft.com/azure/active-directory/devices/overview)

Weitere Informationen zum Aktivieren des Geräterückschreibens für Geräte finden Sie unter ["Geräterückschreiben aktivieren".](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)
