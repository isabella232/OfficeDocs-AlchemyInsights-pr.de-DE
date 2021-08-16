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
ms.openlocfilehash: 78af4dc8cfe38586dcec8d01b72170b56d98fa27860489bf2ca9544f32210c37
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101949"
---
# <a name="device-writeback"></a>Geräterückschreiben

Das Geräterückschreiben wird in den folgenden Szenarien verwendet:

- Aktivieren [Windows Hello for Business mithilfe einer Hybridbereitstellung mit Zertifikatvertrauensstellung](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Aktivieren des bedingten Zugriffs basierend auf Geräten für ADFS (2012 R2 oder höher) geschützte Anwendungen (Vertrauensstellungen der vertrauenden Seite)

    > [!NOTE]
    > Für das Geräterückschreiben ist ein Abonnement für Azure AD Premium erforderlich.

Dies bietet zusätzliche Sicherheit und Sicherheit, dass der Zugriff auf Anwendungen nur vertrauenswürdigen Geräten gewährt wird. Weitere Informationen zum bedingten Zugriff finden Sie unter [Verwalten von Risiken mit bedingtem Zugriff](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) und Einrichten des lokalen [bedingten Zugriffs mit Azure Active Directory Geräteregistrierung.](https://docs.microsoft.com/azure/active-directory/devices/overview)

Weitere Informationen zum Aktivieren des Geräterückschreibens für Geräte finden Sie unter Aktivieren des [Geräterückschreibens.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)
