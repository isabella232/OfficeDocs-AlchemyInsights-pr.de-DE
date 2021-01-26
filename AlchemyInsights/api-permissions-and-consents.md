---
title: API-Berechtigungen und Zustimmung
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951894"
---
# <a name="api-permissions-and-consent"></a>API-Berechtigungen und Zustimmung

Anwendungen, die mit Microsoft Identity Platform integriert werden, folgen einem Autorisierungsmodell, mit dem Benutzer und Administratoren steuern können, wie auf Daten zugegriffen werden kann. Die Implementierung des Autorisierungsmodells wurde auf dem Microsoft Identity Platform-Endpunkt aktualisiert. Es ändert die Art und Weise, wie eine App mit der Microsoft Identity Platform interagieren muss. [Berechtigungen und Zustimmungen im Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) Platform-Endpunkt umfassen die grundlegenden Konzepte dieses Autorisierungsmodells, einschließlich Bereiche, Berechtigungen und Zustimmung.

Das [Azure Active Directory (Azure AD)-Zustimmungsframework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) erleichtert die Entwicklung von mehr mandanteneigenen Web- und systemeigenen Clientanwendungen. Diese Anwendungen ermöglichen die Anmeldung über Benutzerkonten von einem Azure AD-Mandanten, der sich von dem, in dem die Anwendung registriert ist, unterscheiden. Sie müssen möglicherweise zusätzlich zu Ihren eigenen Web-APIs auch auf Web-APIs wie die Microsoft Graph-API (für den Zugriff auf Azure AD, Intune und Dienste in Microsoft 365) und die APIs anderer Microsoft-Dienste zugreifen.

