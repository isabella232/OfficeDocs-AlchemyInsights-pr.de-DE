---
title: Single-Sign für Azure Active Directory-beigetretene Geräte aktiviert
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403797"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Einmaliges Anmelden für Azure Active Directory-beigetretene Geräte

Wenn Sie über eine lokale Active Directory (AD)-Umgebung verfügen und Ihre mit der AD-Domäne beigetretenen Computer zu Azure AD hinzufügen möchten, können Sie dies erreichen, indem Sie azure AD hybrid beitreten. [How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.

[Konfigurieren von In Azure AD beigetretenen Geräten für lokale Single-Sign On mithilfe von Windows Hello for Business](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Probleme mit dem primären Aktualisierungstoken (Primary Refresh Token, PRT)** Ein primäres Aktualisierungstoken (Primary Refresh Token, PRT) ist ein Schlüsselartefakte der Azure AD-Authentifizierung auf Windows 10-, Windows Server 2016- und höher-, iOS- und Android-Geräten. Es handelt sich um ein JSON-Webtoken (JWT), das speziell für Tokenbroker von Microsoft first party ausgegeben wurde, um einmaliges Anmelden (Single Sign-On, SSO) für die Anwendungen zu aktivieren, die auf diesen Geräten verwendet werden. [Unter Was ist ein primäres Aktualisierungstoken?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)stellen wir Details dazu zur Verfügung, wie ein PRT auf Windows 10-Geräten ausgegeben, verwendet und geschützt wird.

**WamDefaultSet: JA und AzureADPrt: JA** Diese Felder geben an, ob sich der Benutzer erfolgreich bei Azure AD authentifiziert hat, wenn er sich beim Gerät anmeldet. Wenn die Werte **NO sind,** kann dies fällig sein:

- Ungültiger Speicherschlüssel im TPM, das dem Gerät bei der Registrierung zugeordnet ist (überprüfen Sie den KeySignTest, während Sie mit erhöhten Rechten ausgeführt werden).
- Alternative Anmelde-ID
- HTTP-Proxy nicht gefunden

Behandeln von Problemen mit Geräten mithilfe des Befehls dsregcmd – [SSO-Status](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
