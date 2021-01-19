---
title: Probleme mit der Administrator zustimmung
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49888302"
---
# <a name="admin-consent-issues"></a>Probleme mit der Administrator zustimmung

1. Aktivieren Sie den [Workflow für die Administratorgenehmigung,](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) damit Benutzer die Administratorgenehmigung direkt über den Zustimmungsbildschirm anfordern können.

1. Wenn während des Zustimmungsprozesses unerwartete Fehler angezeigt werden, finden Sie in diesem Artikel Informationen zur Problembehandlung: Unerwarteter Fehler bei der Zustimmung zu [einer Anwendung.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)

1. Erfahren Sie mehr über die Administrator-Zustimmung [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) auf der [Microsoft Identity Platform,](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)wie die Zustimmungsaufforderung funktioniert und wie Sie eine Anforderung für die [mandantenweite Administrator zustimmung auswerten.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)

1. Anwendungen, die in die Microsoft Identity Platform integriert werden, folgen einem Autorisierungsmodell, mit dem Benutzer und Administratoren steuern können, wie auf Daten zugegriffen werden kann. Die Implementierung des Autorisierungsmodells wurde auf dem Microsoft Identity Platform-Endpunkt aktualisiert und ändert, wie eine App mit der Microsoft Identity Platform interagieren muss. Eine Übersicht über dieses Autorisierungsmodell, einschließlich Bereiche, Berechtigungen und Zustimmung, finden Sie unter "Berechtigungen und Zustimmung" im [Microsoft Identity](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) Platform-Endpunkt.